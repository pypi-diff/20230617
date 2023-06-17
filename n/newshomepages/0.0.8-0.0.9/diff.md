# Comparing `tmp/newshomepages-0.0.8.tar.gz` & `tmp/newshomepages-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newshomepages-0.0.8.tar", last modified: Wed Nov 16 21:30:51 2022, max compression
+gzip compressed data, was "newshomepages-0.0.9.tar", last modified: Fri Nov 18 20:40:16 2022, max compression
```

## Comparing `newshomepages-0.0.8.tar` & `newshomepages-0.0.9.tar`

### file list

```diff
@@ -1,626 +1,624 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.031381 newshomepages-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/ISSUE_TEMPLATE/add-a-site.md
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/ISSUE_TEMPLATE/report-a-broken-site.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.939380 newshomepages-0.0.8/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/actions/accessibility/
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/accessibility/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/actions/archive/
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/archive/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/actions/batch/
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/batch/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/actions/discord/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/discord/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/.github/actions/hyperlinks/
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/hyperlinks/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/install/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/install/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/lighthouse/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/lighthouse/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/mosaic/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/mosaic/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/screenshot/
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/screenshot/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/slack/
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/slack/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/telegram/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/telegram/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/tweet/
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/tweet/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/upload/
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/upload/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/actions/wayback/
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/actions/wayback/action.yml
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.951381 newshomepages-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/accessibility-report.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-ajc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-1.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-10.yml
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-3.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-4.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-5.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-6.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-7.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-8.yml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-all-batch-9.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-baltimoresun.yml
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-bundle.yml
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-country.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-globeandmail.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-latimes.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/archive-single-site.yml
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/bln.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/performance-report.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6086 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/reusable-archive-batch-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7812 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/reusable-archive-bundle-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6037 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/reusable-archive-country-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/reusable-archive-single-site-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/site.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/status-report.yml
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.github/workflows/twitter-list.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-11-16 21:30:16.000000 newshomepages-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5213 2022-11-16 21:30:16.000000 newshomepages-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-16 21:30:16.000000 newshomepages-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-16 21:30:16.000000 newshomepages-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-16 21:30:16.000000 newshomepages-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-11-16 21:30:16.000000 newshomepages-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-11-16 21:30:51.031381 newshomepages-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-11-16 21:30:16.000000 newshomepages-0.0.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)   223800 2022-11-16 21:30:16.000000 newshomepages-0.0.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-16 21:30:16.000000 newshomepages-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-11-16 21:30:16.000000 newshomepages-0.0.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/altair_theme.py
--rw-r--r--   0 runner    (1001) docker     (121)    15728 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/analyze.py
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/discorder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/newshomepages/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.943380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ar/
--rw-r--r--   0 runner    (1001) docker     (121)    20357 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ar/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/be/
--rw-r--r--   0 runner    (1001) docker     (121)    39687 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/be/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/bg/
--rw-r--r--   0 runner    (1001) docker     (121)    11379 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/bg/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/bn/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/bn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ca/
--rw-r--r--   0 runner    (1001) docker     (121)    11265 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ca/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/cs/
--rw-r--r--   0 runner    (1001) docker     (121)    33283 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/cs/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/da/
--rw-r--r--   0 runner    (1001) docker     (121)    32176 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/da/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/de/
--rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/de/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/el/
--rw-r--r--   0 runner    (1001) docker     (121)    35861 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/el/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/en/
--rw-r--r--   0 runner    (1001) docker     (121)    31529 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/en/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/es/
--rw-r--r--   0 runner    (1001) docker     (121)    33470 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/es/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/es_419/
--rw-r--r--   0 runner    (1001) docker     (121)    33470 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/es_419/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/et/
--rw-r--r--   0 runner    (1001) docker     (121)    16155 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/et/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fa/
--rw-r--r--   0 runner    (1001) docker     (121)    24231 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fa/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fi/
--rw-r--r--   0 runner    (1001) docker     (121)    32862 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fil/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fil/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fr/
--rw-r--r--   0 runner    (1001) docker     (121)    34308 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/he/
--rw-r--r--   0 runner    (1001) docker     (121)    35288 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/he/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hi/
--rw-r--r--   0 runner    (1001) docker     (121)    21672 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hr/
--rw-r--r--   0 runner    (1001) docker     (121)    32967 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hu/
--rw-r--r--   0 runner    (1001) docker     (121)    34371 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hu/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hy/
--rw-r--r--   0 runner    (1001) docker     (121)    10692 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hy/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/id/
--rw-r--r--   0 runner    (1001) docker     (121)    32258 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/id/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/it/
--rw-r--r--   0 runner    (1001) docker     (121)    33384 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/it/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ja/
--rw-r--r--   0 runner    (1001) docker     (121)    37387 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ja/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/kn/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/kn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ko/
--rw-r--r--   0 runner    (1001) docker     (121)    33544 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ko/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/lt/
--rw-r--r--   0 runner    (1001) docker     (121)    21630 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/lt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/lv/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/lv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/mk-MK/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/mk-MK/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ms/
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ms/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/nb/
--rw-r--r--   0 runner    (1001) docker     (121)    20450 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/nb/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/nl/
--rw-r--r--   0 runner    (1001) docker     (121)    33052 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/nl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pl/
--rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (121)    33333 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pt_BR/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (121)    33264 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pt_PT/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ro/
--rw-r--r--   0 runner    (1001) docker     (121)    33424 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ro/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ru/
--rw-r--r--   0 runner    (1001) docker     (121)    40337 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ru/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sk/
--rw-r--r--   0 runner    (1001) docker     (121)    33371 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sl/
--rw-r--r--   0 runner    (1001) docker     (121)    32933 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sr/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sr-Latn/
--rw-r--r--   0 runner    (1001) docker     (121)    31450 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sv/
--rw-r--r--   0 runner    (1001) docker     (121)    19829 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ta/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ta/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/te/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/te/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/th/
--rw-r--r--   0 runner    (1001) docker     (121)    22289 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/th/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/tr/
--rw-r--r--   0 runner    (1001) docker     (121)    33471 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/tr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/uk/
--rw-r--r--   0 runner    (1001) docker     (121)    39572 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/uk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.959380 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/vi/
--rw-r--r--   0 runner    (1001) docker     (121)    35067 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/vi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.963381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (121)    31240 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/zh_CN/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.963381 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (121)    31840 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/zh_TW/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.943380 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.963381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/
--rw-r--r--   0 runner    (1001) docker     (121)    22094 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/alert-popup.css
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/c3.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.963381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     2573 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/dark.css
--rw-r--r--   0 runner    (1001) docker     (121)    16789 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css
--rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css
--rw-r--r--   0 runner    (1001) docker     (121)    11392 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css
--rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/fonts.css
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/layout.css
--rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/log.css
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/main.css
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/nanobar.css
--rw-r--r--   0 runner    (1001) docker     (121)    54145 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.963381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    66004 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    66708 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    65764 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.963381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-off-19.png
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-off-38.png
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-on-19.png
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-on-38.png
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/gray-19.png
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/gray-38.png
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-128.png
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-16.png
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-19.png
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-38.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.967381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (121)    23194 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/app-store.svg
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/avatar.svg
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/checked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/chrome.svg
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/cross.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/dropbox.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9086 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     6547 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/filters.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5451 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/google-play.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14249 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/hero-green.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11250 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/hero-red.svg
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/link.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo-shield.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo_adguard.svg
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/reload-ico.svg
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/shield.svg
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/tick.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/toggler-bg.svg
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/trash.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.967381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/js/
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/js/preload-theme.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.943380 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.967381 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/libs/scriptlets/
--rw-r--r--   0 runner    (1001) docker     (121)   141578 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.967381 newshomepages-0.0.8/newshomepages/extensions/adguard/content-script/
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/content-script/subscribe.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.995381 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/
--rw-r--r--   0 runner    (1001) docker     (121)  1206317 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)    73188 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_10.txt
--rw-r--r--   0 runner    (1001) docker     (121)   313462 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_11.txt
--rw-r--r--   0 runner    (1001) docker     (121)    94026 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_12.txt
--rw-r--r--   0 runner    (1001) docker     (121)   402899 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_13.txt
--rw-r--r--   0 runner    (1001) docker     (121)  2213341 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_14.txt
--rw-r--r--   0 runner    (1001) docker     (121)   928335 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_15.txt
--rw-r--r--   0 runner    (1001) docker     (121)   774091 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_16.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35060 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_17.txt
--rw-r--r--   0 runner    (1001) docker     (121)  4655227 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)   735758 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_224.txt
--rw-r--r--   0 runner    (1001) docker     (121)   914459 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_3.txt
--rw-r--r--   0 runner    (1001) docker     (121)   585242 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_4.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19066 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_5.txt
--rw-r--r--   0 runner    (1001) docker     (121)   496599 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_6.txt
--rw-r--r--   0 runner    (1001) docker     (121)   271134 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_7.txt
--rw-r--r--   0 runner    (1001) docker     (121)    69106 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_8.txt
--rw-r--r--   0 runner    (1001) docker     (121)   237431 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_9.txt
--rw-r--r--   0 runner    (1001) docker     (121)   483303 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)    67127 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_10.txt
--rw-r--r--   0 runner    (1001) docker     (121)   256792 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_11.txt
--rw-r--r--   0 runner    (1001) docker     (121)    71645 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_12.txt
--rw-r--r--   0 runner    (1001) docker     (121)   363915 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_13.txt
--rw-r--r--   0 runner    (1001) docker     (121)  1223256 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_14.txt
--rw-r--r--   0 runner    (1001) docker     (121)   899376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_15.txt
--rw-r--r--   0 runner    (1001) docker     (121)   341390 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_16.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21554 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_17.txt
--rw-r--r--   0 runner    (1001) docker     (121)  1640295 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)   710272 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_224.txt
--rw-r--r--   0 runner    (1001) docker     (121)   806171 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_3.txt
--rw-r--r--   0 runner    (1001) docker     (121)   361755 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_4.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8985 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_5.txt
--rw-r--r--   0 runner    (1001) docker     (121)   193843 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_6.txt
--rw-r--r--   0 runner    (1001) docker     (121)   249182 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_7.txt
--rw-r--r--   0 runner    (1001) docker     (121)    58256 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_8.txt
--rw-r--r--   0 runner    (1001) docker     (121)   191331 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_9.txt
--rw-r--r--   0 runner    (1001) docker     (121)    51441 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filters.json
--rw-r--r--   0 runner    (1001) docker     (121)   799078 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filters_i18n.json
--rw-r--r--   0 runner    (1001) docker     (121)  1545375 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/filters/local_script_rules.json
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.007381 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/ad-blocked.html
--rw-r--r--   0 runner    (1001) docker     (121)   177876 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/ad-blocked.js
--rw-r--r--   0 runner    (1001) docker     (121)   650939 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/assistant.js
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/background.html
--rw-r--r--   0 runner    (1001) docker     (121)  3189967 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/background.js
--rw-r--r--   0 runner    (1001) docker     (121)    15084 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/content-script-end.js
--rw-r--r--   0 runner    (1001) docker     (121)   288034 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/content-script-start.js
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html
--rw-r--r--   0 runner    (1001) docker     (121)    19803 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools.html
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools.js
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filter-download.html
--rw-r--r--   0 runner    (1001) docker     (121)    62185 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filter-download.js
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filtering-log.html
--rw-r--r--   0 runner    (1001) docker     (121)  1408341 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filtering-log.js
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html
--rw-r--r--   0 runner    (1001) docker     (121)   582536 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/options.html
--rw-r--r--   0 runner    (1001) docker     (121)  1079105 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/options.js
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/popup.html
--rw-r--r--   0 runner    (1001) docker     (121)  1072410 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/popup.js
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/safebrowsing.html
--rw-r--r--   0 runner    (1001) docker     (121)   177879 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/safebrowsing.js
--rw-r--r--   0 runner    (1001) docker     (121)    62942 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/pages/thankyou.js
--rw-r--r--   0 runner    (1001) docker     (121)     7449 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.007381 newshomepages-0.0.8/newshomepages/extensions/adguard/shared/
--rw-r--r--   0 runner    (1001) docker     (121)  1063347 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/shared/editor.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.007381 newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/
--rw-r--r--   0 runner    (1001) docker     (121)   176243 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/mobx.js
--rw-r--r--   0 runner    (1001) docker     (121)   135893 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/react.js
--rw-r--r--   0 runner    (1001) docker     (121)    50712 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/xstate.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.943380 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.011381 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/1x1-transparent.gif
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/2x2-transparent.png
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/32x32-transparent.png
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/3x2-transparent.png
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js
--rw-r--r--   0 runner    (1001) docker     (121)     9125 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html
--rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js
--rw-r--r--   0 runner    (1001) docker     (121)     5377 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (121)    18549 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js
--rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js
--rw-r--r--   0 runner    (1001) docker     (121)     6722 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js
--rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopcss.css
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopframe.html
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjs.js
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjson.json
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3
--rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/nooptext.js
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast02.xml
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast03.xml
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast04.xml
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvmap01.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js
--rw-r--r--   0 runner    (1001) docker     (121)     3509 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js
--rw-r--r--   0 runner    (1001) docker     (121)     3988 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js
--rw-r--r--   0 runner    (1001) docker     (121)     4200 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.011381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.011381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ar/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ar/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/be/
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/be/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/bg/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/bg/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/cs/
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/cs/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/da/
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/da/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/de/
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/de/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/en/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/en/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/es/
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/es/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/et/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/et/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fa/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fa/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fi/
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fr/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/he/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/he/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hr/
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hu/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hu/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hy/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hy/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/id/
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/id/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/it/
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/it/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ja/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ja/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ko/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ko/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/lt/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/lt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/nl/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/nl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/no/
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/no/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pl/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pt/
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pt-PT/
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ro/
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ro/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ru/
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ru/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sk/
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sl/
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sr/
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sv/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/tr/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/tr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/uk/
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/uk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/vi/
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/vi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/zh/
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/zh/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/zh-TW/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.015381 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_installed.png
--rw-r--r--   0 runner    (1001) docker     (121)     7769 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/content-script.js
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/options.js
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/popup.css
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/popup.html
--rw-r--r--   0 runner    (1001) docker     (121)   158820 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/adguardextra/userscript.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.947380 newshomepages-0.0.8/newshomepages/extensions/singlefile/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.019381 newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/
--rw-r--r--   0 runner    (1001) docker     (121)    25444 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file-bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (121)    21126 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file-frames.js
--rw-r--r--   0 runner    (1001) docker     (121)     8419 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file-hooks-frames.js
--rw-r--r--   0 runner    (1001) docker     (121)   296387 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file.js
--rw-r--r--   0 runner    (1001) docker     (121)    18323 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/hyperlinks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6242 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/rss.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (121)    23002 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/site.py
--rw-r--r--   0 runner    (1001) docker     (121)     4239 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.019381 newshomepages-0.0.8/newshomepages/sources/
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/bundles.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:51.031381 newshomepages-0.0.8/newshomepages/sources/javascript/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/20minutes.js
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/_fiquemsabendo.js
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/abc_es.js
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/andscape.js
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/arthasarokar.js
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/asahi.js
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/baltimorebanner.js
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/baltimoremag.js
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/baltimoresun.js
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/bariweiss.js
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/bbc.js
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/bloombergjapan.js
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/bonginoreport.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/breitbartnews.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/calgaryherald.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/cbcnews.js
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/chess24com.js
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/chicagotribune.js
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/civilbeat.js
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/cnn.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/crucessunnews.js
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/daily_record.js
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/dailycaller.js
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/diariope.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/dmregister.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/drudge.js
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/el_universal_mx.js
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/elcorreo_com.js
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/eltiempo.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/financialpost.js
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/firstthingsmag.js
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/fortunemagazine.js
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/foxnews.js
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/france24.js
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/france24_en.js
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/franceinfo.js
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/frednewspost.js
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/ft.js
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/gazettedotcom.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/gbpressgazette.js
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/georgiastraight.js
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/globalnews.js
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/globeandmail.js
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/gridnews.js
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/guardian.js
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/htrnews.js
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/independent.js
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/izvestia_ru.js
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/jdemontreal.js
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/jessicavalenti.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/journalsentinel.js
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/kcautv.js
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/kccinews.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/kpbs.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/kpcc.js
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/laist.js
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/lajornada.js
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/larazon_es.js
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/latimes.js
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/lavozdegalicia.js
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/le_figaro.js
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/le_parisien.js
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/ledevoir.js
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/lehuffpost.js
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/lemonde_en.js
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/lemondefr.js
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/libe.js
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/lp_lapresse.js
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/maroelamedia.js
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/mediapart.js
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/moreperfectus.js
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/motherjones.js
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/msnbc.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/mtlgazette.js
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/mtnstspotlight.js
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/nationalpost.js
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/nbcnews.js
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/news_letter.js
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/newshour.js
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/nhk_news.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/nikkei.js
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/ntdaily.js
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/nytimes.js
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/oann.js
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/occrp.js
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/openvallejo.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/ottawacitizen.js
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/pajaropolitico.js
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/pioneerpress.js
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/platformer.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/postcrescent.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/presscitizen.js
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/propublica.js
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/publicintegrity.js
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/pulitzercenter.js
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/qctimes.js
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/realdailywire.js
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/rfi.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/sahanjournal.js
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/sankei_news.js
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/sdut.js
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/seikyoofficial.js
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/sfchronicle.js
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/sowetanlive.js
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/sputnikint.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/startribune.js
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/statnews.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/stevenspointjrl.js
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/teamtrace.js
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/telegraph.js
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/theathletic.js
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thebabylonbee.js
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/theblaze.js
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thedbk.js
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thedispatch.js
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/theeconomist.js
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thehilltimes.js
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/theonion.js
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thesun.js
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thetimes.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thetorontosun.js
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thetriibe.js
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/thewrap.js
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/timeslive.js
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/torontostar.js
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/usatoday.js
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/vancouversun.js
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/vcstar.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/votebeatus.js
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/vryeweekblad.js
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/javascript/wcfcourier.js
--rw-r--r--   0 runner    (1001) docker     (121)   109271 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/sources/sites.csv
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/telegrammer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14178 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/tweet.py
--rw-r--r--   0 runner    (1001) docker     (121)    19677 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2022-11-16 21:30:20.000000 newshomepages-0.0.8/newshomepages/wayback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 21:30:50.955381 newshomepages-0.0.8/newshomepages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-11-16 21:30:45.000000 newshomepages-0.0.8/newshomepages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    26237 2022-11-16 21:30:50.000000 newshomepages-0.0.8/newshomepages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 21:30:45.000000 newshomepages-0.0.8/newshomepages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-11-16 21:30:45.000000 newshomepages-0.0.8/newshomepages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 21:30:45.000000 newshomepages-0.0.8/newshomepages.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-16 21:30:45.000000 newshomepages-0.0.8/newshomepages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-16 21:30:45.000000 newshomepages-0.0.8/newshomepages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-11-16 21:30:51.031381 newshomepages-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-11-16 21:30:20.000000 newshomepages-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.313545 newshomepages-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/ISSUE_TEMPLATE/add-a-site.md
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/ISSUE_TEMPLATE/report-a-broken-site.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.237545 newshomepages-0.0.9/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/.github/actions/accessibility/
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/accessibility/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/archive/
+-rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/archive/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/batch/
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/batch/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/discord/
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/discord/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/hyperlinks/
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/hyperlinks/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/install/
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/install/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/lighthouse/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/lighthouse/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/mosaic/
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/mosaic/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/screenshot/
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/screenshot/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/slack/
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/slack/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/telegram/
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/telegram/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/tweet/
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/tweet/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/upload/
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/upload/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/actions/wayback/
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/actions/wayback/action.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.245545 newshomepages-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/accessibility-report.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-ajc.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-10.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-2.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-3.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-4.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-5.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-6.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-7.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-8.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-all-batch-9.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-baltimoresun.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-bundle.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-globeandmail.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-latimes.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/archive-single-site.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/bln.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/performance-report.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6086 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/reusable-archive-batch-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/reusable-archive-single-site-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/site.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.github/workflows/status-report.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-11-18 20:39:43.000000 newshomepages-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5213 2022-11-18 20:39:43.000000 newshomepages-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-18 20:39:43.000000 newshomepages-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-18 20:39:43.000000 newshomepages-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-18 20:39:43.000000 newshomepages-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-11-18 20:39:43.000000 newshomepages-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-11-18 20:40:16.313545 newshomepages-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-18 20:39:43.000000 newshomepages-0.0.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (121)   224140 2022-11-18 20:39:43.000000 newshomepages-0.0.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-18 20:39:43.000000 newshomepages-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-11-18 20:39:43.000000 newshomepages-0.0.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-18 20:39:45.000000 newshomepages-0.0.9/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/altair_theme.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15728 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5795 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/discorder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/newshomepages/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.237545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ar/
+-rw-r--r--   0 runner    (1001) docker     (121)    20357 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ar/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/be/
+-rw-r--r--   0 runner    (1001) docker     (121)    39687 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/be/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/bg/
+-rw-r--r--   0 runner    (1001) docker     (121)    11379 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/bg/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/bn/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/bn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ca/
+-rw-r--r--   0 runner    (1001) docker     (121)    11265 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ca/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/cs/
+-rw-r--r--   0 runner    (1001) docker     (121)    33283 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/cs/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/da/
+-rw-r--r--   0 runner    (1001) docker     (121)    32176 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/da/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/de/
+-rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/de/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/el/
+-rw-r--r--   0 runner    (1001) docker     (121)    35861 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/el/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/en/
+-rw-r--r--   0 runner    (1001) docker     (121)    31529 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/en/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/es/
+-rw-r--r--   0 runner    (1001) docker     (121)    33470 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/es/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/es_419/
+-rw-r--r--   0 runner    (1001) docker     (121)    33470 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/es_419/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/et/
+-rw-r--r--   0 runner    (1001) docker     (121)    16155 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/et/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fa/
+-rw-r--r--   0 runner    (1001) docker     (121)    24231 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fa/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fi/
+-rw-r--r--   0 runner    (1001) docker     (121)    32862 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fil/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fil/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fr/
+-rw-r--r--   0 runner    (1001) docker     (121)    34308 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/he/
+-rw-r--r--   0 runner    (1001) docker     (121)    35288 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/he/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hi/
+-rw-r--r--   0 runner    (1001) docker     (121)    21672 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hr/
+-rw-r--r--   0 runner    (1001) docker     (121)    32967 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hu/
+-rw-r--r--   0 runner    (1001) docker     (121)    34371 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hu/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hy/
+-rw-r--r--   0 runner    (1001) docker     (121)    10692 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hy/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/id/
+-rw-r--r--   0 runner    (1001) docker     (121)    32258 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/id/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/it/
+-rw-r--r--   0 runner    (1001) docker     (121)    33384 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/it/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ja/
+-rw-r--r--   0 runner    (1001) docker     (121)    37387 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ja/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/kn/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/kn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ko/
+-rw-r--r--   0 runner    (1001) docker     (121)    33544 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ko/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/lt/
+-rw-r--r--   0 runner    (1001) docker     (121)    21630 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/lt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/lv/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/lv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/mk-MK/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/mk-MK/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ms/
+-rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ms/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/nb/
+-rw-r--r--   0 runner    (1001) docker     (121)    20450 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/nb/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/nl/
+-rw-r--r--   0 runner    (1001) docker     (121)    33052 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/nl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pl/
+-rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (121)    33333 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pt_BR/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (121)    33264 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pt_PT/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ro/
+-rw-r--r--   0 runner    (1001) docker     (121)    33424 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ro/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ru/
+-rw-r--r--   0 runner    (1001) docker     (121)    40337 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ru/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sk/
+-rw-r--r--   0 runner    (1001) docker     (121)    33371 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sl/
+-rw-r--r--   0 runner    (1001) docker     (121)    32933 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sr/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sr-Latn/
+-rw-r--r--   0 runner    (1001) docker     (121)    31450 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sv/
+-rw-r--r--   0 runner    (1001) docker     (121)    19829 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ta/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ta/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/te/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/te/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/th/
+-rw-r--r--   0 runner    (1001) docker     (121)    22289 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/th/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/tr/
+-rw-r--r--   0 runner    (1001) docker     (121)    33471 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/tr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/uk/
+-rw-r--r--   0 runner    (1001) docker     (121)    39572 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/uk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/vi/
+-rw-r--r--   0 runner    (1001) docker     (121)    35067 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/vi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (121)    31240 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/zh_CN/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (121)    31840 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/zh_TW/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.237545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (121)    22094 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/alert-popup.css
+-rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/c3.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.253545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2573 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/dark.css
+-rw-r--r--   0 runner    (1001) docker     (121)    16789 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css
+-rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css
+-rw-r--r--   0 runner    (1001) docker     (121)    11392 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css
+-rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css
+-rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/layout.css
+-rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/log.css
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/nanobar.css
+-rw-r--r--   0 runner    (1001) docker     (121)    54145 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.257545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)    66004 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    66708 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    65764 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.257545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-off-19.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-off-38.png
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-on-19.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-on-38.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/gray-19.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/gray-38.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-128.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-19.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-38.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.257545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    23194 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/app-store.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/avatar.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/checked.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/chrome.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/dropbox.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     9086 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     6547 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/filters.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5451 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/google-play.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    14249 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/hero-green.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    11250 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/hero-red.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/link.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo-shield.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo_adguard.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/reload-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/shield.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/tick.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/toggler-bg.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/trash.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.257545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/js/preload-theme.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.237545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/libs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.257545 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/libs/scriptlets/
+-rw-r--r--   0 runner    (1001) docker     (121)   141578 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.257545 newshomepages-0.0.9/newshomepages/extensions/adguard/content-script/
+-rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/content-script/subscribe.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.281545 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)  1206317 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    73188 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   313462 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_11.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    94026 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_12.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   402899 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_13.txt
+-rw-r--r--   0 runner    (1001) docker     (121)  2213341 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_14.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   928335 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_15.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   774091 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_16.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    35060 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_17.txt
+-rw-r--r--   0 runner    (1001) docker     (121)  4655227 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   735758 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_224.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   914459 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   585242 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19066 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   496599 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   271134 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    69106 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_8.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   237431 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_9.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   483303 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    67127 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_10.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   256792 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_11.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    71645 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_12.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   363915 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_13.txt
+-rw-r--r--   0 runner    (1001) docker     (121)  1223256 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_14.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   899376 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_15.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   341390 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_16.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21554 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_17.txt
+-rw-r--r--   0 runner    (1001) docker     (121)  1640295 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   710272 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_224.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   806171 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   361755 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8985 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   193843 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   249182 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_7.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    58256 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_8.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   191331 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_9.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    51441 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filters.json
+-rw-r--r--   0 runner    (1001) docker     (121)   799078 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filters_i18n.json
+-rw-r--r--   0 runner    (1001) docker     (121)  1545375 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/filters/local_script_rules.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.293545 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/ad-blocked.html
+-rw-r--r--   0 runner    (1001) docker     (121)   177876 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/ad-blocked.js
+-rw-r--r--   0 runner    (1001) docker     (121)   650939 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-18 20:39:45.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/background.html
+-rw-r--r--   0 runner    (1001) docker     (121)  3189967 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/background.js
+-rw-r--r--   0 runner    (1001) docker     (121)    15084 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/content-script-end.js
+-rw-r--r--   0 runner    (1001) docker     (121)   288034 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/content-script-start.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (121)    19803 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools.js
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filter-download.html
+-rw-r--r--   0 runner    (1001) docker     (121)    62185 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filter-download.js
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filtering-log.html
+-rw-r--r--   0 runner    (1001) docker     (121)  1408341 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filtering-log.js
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html
+-rw-r--r--   0 runner    (1001) docker     (121)   582536 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/options.html
+-rw-r--r--   0 runner    (1001) docker     (121)  1079105 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/options.js
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/popup.html
+-rw-r--r--   0 runner    (1001) docker     (121)  1072410 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/popup.js
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/safebrowsing.html
+-rw-r--r--   0 runner    (1001) docker     (121)   177879 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/safebrowsing.js
+-rw-r--r--   0 runner    (1001) docker     (121)    62942 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/pages/thankyou.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7449 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.293545 newshomepages-0.0.9/newshomepages/extensions/adguard/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)  1063347 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/shared/editor.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.293545 newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/
+-rw-r--r--   0 runner    (1001) docker     (121)   176243 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/mobx.js
+-rw-r--r--   0 runner    (1001) docker     (121)   135893 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/react.js
+-rw-r--r--   0 runner    (1001) docker     (121)    50712 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/xstate.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.237545 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/1x1-transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/2x2-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/32x32-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/3x2-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9125 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html
+-rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5377 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (121)    18549 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6722 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopcss.css
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopframe.html
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjs.js
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjson.json
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3
+-rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/nooptext.js
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast02.xml
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast03.xml
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast04.xml
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvmap01.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3509 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3988 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4200 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ar/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ar/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/be/
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/be/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/bg/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/bg/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/cs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/cs/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.297545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/da/
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/da/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/de/
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/de/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/en/
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/en/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/es/
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/es/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/et/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/et/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fa/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fa/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fi/
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fr/
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/he/
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/he/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hr/
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hu/
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hu/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hy/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hy/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/id/
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/id/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/it/
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/it/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ja/
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ja/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ko/
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ko/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/lt/
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/lt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/nl/
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/nl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/no/
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/no/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pt/
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pt-PT/
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ro/
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ro/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ru/
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ru/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sr/
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sv/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/tr/
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/tr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/uk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/uk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/vi/
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/vi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/zh/
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/zh/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/zh-TW/
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_installed.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7769 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/content-script.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/options.js
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/popup.css
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/popup.html
+-rw-r--r--   0 runner    (1001) docker     (121)   158820 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/adguardextra/userscript.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.241545 newshomepages-0.0.9/newshomepages/extensions/singlefile/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/
+-rw-r--r--   0 runner    (1001) docker     (121)    25444 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file-bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (121)    21126 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file-frames.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8419 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file-hooks-frames.js
+-rw-r--r--   0 runner    (1001) docker     (121)   296387 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file.js
+-rw-r--r--   0 runner    (1001) docker     (121)    18323 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/hyperlinks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4955 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6242 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/rss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23002 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/site.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4239 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.301545 newshomepages-0.0.9/newshomepages/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/bundles.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.313545 newshomepages-0.0.9/newshomepages/sources/javascript/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/20minutes.js
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/_fiquemsabendo.js
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/abc_es.js
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/andscape.js
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/arthasarokar.js
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/asahi.js
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/baltimorebanner.js
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/baltimoremag.js
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/baltimoresun.js
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/bariweiss.js
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/bbc.js
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/bloombergjapan.js
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/bonginoreport.js
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/breitbartnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/calgaryherald.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/cbcnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/chess24com.js
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/chicagotribune.js
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/civilbeat.js
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/cnn.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/crucessunnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/daily_record.js
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/dailycaller.js
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/diariope.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/dmregister.js
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/drudge.js
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/el_universal_mx.js
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/elcorreo_com.js
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/eltiempo.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/financialpost.js
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/firstthingsmag.js
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/fortunemagazine.js
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/foxnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/france24.js
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/france24_en.js
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/franceinfo.js
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/frednewspost.js
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/ft.js
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/gazettedotcom.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/gbpressgazette.js
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/georgiastraight.js
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/globalnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/globeandmail.js
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/gridnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/guardian.js
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/htrnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/independent.js
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/izvestia_ru.js
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/jdemontreal.js
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/jessicavalenti.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/journalsentinel.js
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/kcautv.js
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/kccinews.js
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/kpbs.js
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/kpcc.js
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/laist.js
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/lajornada.js
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/larazon_es.js
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/latimes.js
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/lavozdegalicia.js
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/le_figaro.js
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/le_parisien.js
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/ledevoir.js
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/lehuffpost.js
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/lemonde_en.js
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/lemondefr.js
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/libe.js
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/lp_lapresse.js
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/maroelamedia.js
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/mediapart.js
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/moreperfectus.js
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/motherjones.js
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/msnbc.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/mtlgazette.js
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/mtnstspotlight.js
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/nationalpost.js
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/nbcnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/news_letter.js
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/newshour.js
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/nhk_news.js
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/nikkei.js
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/ntdaily.js
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/nytimes.js
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/oann.js
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/occrp.js
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/openvallejo.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/ottawacitizen.js
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/pajaropolitico.js
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/pioneerpress.js
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/platformer.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/postcrescent.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/presscitizen.js
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/propublica.js
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/publicintegrity.js
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/pulitzercenter.js
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/qctimes.js
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/realdailywire.js
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/rfi.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/sahanjournal.js
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/sankei_news.js
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/sdut.js
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/seikyoofficial.js
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/sfchronicle.js
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/sowetanlive.js
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/sputnikint.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/startribune.js
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/statnews.js
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/stevenspointjrl.js
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/teamtrace.js
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/telegraph.js
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/theathletic.js
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thebabylonbee.js
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/theblaze.js
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thedbk.js
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thedispatch.js
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/theeconomist.js
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thehilltimes.js
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/theonion.js
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thesun.js
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thetimes.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thetorontosun.js
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thetriibe.js
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/thewrap.js
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/timeslive.js
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/torontostar.js
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/usatoday.js
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/vancouversun.js
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/vcstar.js
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/votebeatus.js
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/vryeweekblad.js
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/javascript/wcfcourier.js
+-rw-r--r--   0 runner    (1001) docker     (121)   109271 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/sources/sites.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/telegrammer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14178 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/tweet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19677 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3009 2022-11-18 20:39:46.000000 newshomepages-0.0.9/newshomepages/wayback.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 20:40:16.249545 newshomepages-0.0.9/newshomepages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-11-18 20:40:13.000000 newshomepages-0.0.9/newshomepages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    26029 2022-11-18 20:40:16.000000 newshomepages-0.0.9/newshomepages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 20:40:13.000000 newshomepages-0.0.9/newshomepages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2022-11-18 20:40:13.000000 newshomepages-0.0.9/newshomepages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 20:40:13.000000 newshomepages-0.0.9/newshomepages.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-18 20:40:13.000000 newshomepages-0.0.9/newshomepages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-18 20:40:13.000000 newshomepages-0.0.9/newshomepages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 20:39:46.000000 newshomepages-0.0.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 20:40:16.313545 newshomepages-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-11-18 20:39:46.000000 newshomepages-0.0.9/setup.py
```

### Comparing `newshomepages-0.0.8/.github/ISSUE_TEMPLATE/add-a-site.md` & `newshomepages-0.0.9/.github/ISSUE_TEMPLATE/add-a-site.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/accessibility/action.yml` & `newshomepages-0.0.9/.github/actions/accessibility/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/archive/action.yml` & `newshomepages-0.0.9/.github/actions/archive/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/batch/action.yml` & `newshomepages-0.0.9/.github/actions/batch/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/discord/action.yml` & `newshomepages-0.0.9/.github/actions/discord/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/hyperlinks/action.yml` & `newshomepages-0.0.9/.github/actions/hyperlinks/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/install/action.yml` & `newshomepages-0.0.9/.github/actions/install/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/lighthouse/action.yml` & `newshomepages-0.0.9/.github/actions/lighthouse/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/mosaic/action.yml` & `newshomepages-0.0.9/.github/actions/mosaic/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/screenshot/action.yml` & `newshomepages-0.0.9/.github/actions/screenshot/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/slack/action.yml` & `newshomepages-0.0.9/.github/actions/slack/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/telegram/action.yml` & `newshomepages-0.0.9/.github/actions/telegram/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/tweet/action.yml` & `newshomepages-0.0.9/.github/actions/tweet/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/upload/action.yml` & `newshomepages-0.0.9/.github/actions/upload/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/actions/wayback/action.yml` & `newshomepages-0.0.9/.github/actions/wayback/action.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/accessibility-report.yml` & `newshomepages-0.0.9/.github/workflows/accessibility-report.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/archive-ajc.yml` & `newshomepages-0.0.9/.github/workflows/archive-latimes.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-name: "Archive and Slack: Atlanta Journal-Constitution"
+name: "Archive and Slack: Los Angeles Times"
 
 on:
   workflow_dispatch:
-  schedule:
-    - cron: "0 12,19,1 * * *"
+#   schedule:
+#     - cron: "0 13,19,1 * * *"
 
 jobs:
   archive-site:
     name: Archive bundle
     uses: palewire/news-homepages/.github/workflows/reusable-archive-single-site-workflow.yml@main
     with:
-      handle: ajc
+      handle: latimes
     secrets: inherit
 
   newsroom-slack:
     name: Post to newsroom Slack
     runs-on: ubuntu-latest
     timeout-minutes: 15
     needs: [archive-site]
@@ -23,16 +23,16 @@
         name: Checkout
         uses: actions/checkout@v3
 
       - id: slack
         name: Post to Slack
         uses: ./.github/actions/slack
         with:
-          handle: ajc
-          webhook-url: ${{ secrets.SLACK_WEBHOOK_URL_AJC }}
+          handle: latimes
+          webhook-url: ${{ secrets.SLACK_WEBHOOK_URL_LATIMES }}
 
   palewire-slack:
     name: Post to palewire Slack
     runs-on: ubuntu-latest
     timeout-minutes: 15
     needs: [archive-site]
     steps:
@@ -40,9 +40,9 @@
         name: Checkout
         uses: actions/checkout@v3
 
       - id: slack
         name: Post to Slack
         uses: ./.github/actions/slack
         with:
-          handle: ajc
+          handle: latimes
           webhook-url: ${{ secrets.SLACK_WEBHOOK_URL_PALEWIRE }}
```

### Comparing `newshomepages-0.0.8/.github/workflows/archive-all-batch-10.yml` & `newshomepages-0.0.9/.github/workflows/archive-all-batch-10.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/archive-baltimoresun.yml` & `newshomepages-0.0.9/.github/workflows/archive-baltimoresun.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: "Archive and Slack: Baltimore Sun"
 
 on:
   workflow_dispatch:
-  schedule:
-    - cron: "0 10,16,22 * * *"
+#   schedule:
+#     - cron: "0 10,16,22 * * *"
 
 jobs:
   archive-site:
     name: Archive bundle
     uses: palewire/news-homepages/.github/workflows/reusable-archive-single-site-workflow.yml@main
     with:
       handle: baltimoresun
```

### Comparing `newshomepages-0.0.8/.github/workflows/archive-globeandmail.yml` & `newshomepages-0.0.9/.github/workflows/archive-globeandmail.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: "Archive and Slack: Toronto Globe and Mail"
 
 on:
   workflow_dispatch:
-  schedule:
-    - cron: "0 10,16,22 * * *"
+#   schedule:
+#     - cron: "0 10,16,22 * * *"
 
 jobs:
   archive-site:
     name: Archive bundle
     uses: palewire/news-homepages/.github/workflows/reusable-archive-single-site-workflow.yml@main
     with:
       handle: globeandmail
```

### Comparing `newshomepages-0.0.8/.github/workflows/archive-latimes.yaml` & `newshomepages-0.0.9/.github/workflows/archive-ajc.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-name: "Archive and Slack: Los Angeles Times"
+name: "Archive and Slack: Atlanta Journal-Constitution"
 
 on:
   workflow_dispatch:
-  schedule:
-    - cron: "0 13,19,1 * * *"
+#   schedule:
+#     - cron: "0 12,19,1 * * *"
 
 jobs:
   archive-site:
     name: Archive bundle
     uses: palewire/news-homepages/.github/workflows/reusable-archive-single-site-workflow.yml@main
     with:
-      handle: latimes
+      handle: ajc
     secrets: inherit
 
   newsroom-slack:
     name: Post to newsroom Slack
     runs-on: ubuntu-latest
     timeout-minutes: 15
     needs: [archive-site]
@@ -23,16 +23,16 @@
         name: Checkout
         uses: actions/checkout@v3
 
       - id: slack
         name: Post to Slack
         uses: ./.github/actions/slack
         with:
-          handle: latimes
-          webhook-url: ${{ secrets.SLACK_WEBHOOK_URL_LATIMES }}
+          handle: ajc
+          webhook-url: ${{ secrets.SLACK_WEBHOOK_URL_AJC }}
 
   palewire-slack:
     name: Post to palewire Slack
     runs-on: ubuntu-latest
     timeout-minutes: 15
     needs: [archive-site]
     steps:
@@ -40,9 +40,9 @@
         name: Checkout
         uses: actions/checkout@v3
 
       - id: slack
         name: Post to Slack
         uses: ./.github/actions/slack
         with:
-          handle: latimes
+          handle: ajc
           webhook-url: ${{ secrets.SLACK_WEBHOOK_URL_PALEWIRE }}
```

### Comparing `newshomepages-0.0.8/.github/workflows/archive-single-site.yml` & `newshomepages-0.0.9/.github/workflows/archive-single-site.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/bln.yml` & `newshomepages-0.0.9/.github/workflows/bln.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/continuous-deployment.yml` & `newshomepages-0.0.9/.github/workflows/continuous-deployment.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-name: Testing
+name: Test and deploy
+
 on:
   push:
   pull_request:
   workflow_dispatch:
 
+concurrency: 
+  group: ${{ github.workflow }}
+  cancel-in-progress: true
+
 jobs:
   lint-python:
     name: Lint Python code
     runs-on: ubuntu-latest
     steps:
       - id: checkout
         name: Checkout
@@ -63,30 +68,14 @@
         name: Install
         uses: ./.github/actions/install
 
       - id: mypy
         name: mypy
         run: pipenv run mypy ./
 
-  site:
-    name: Build site
-    runs-on: ubuntu-latest
-    steps:
-      - id: checkout
-        name: Checkout
-        uses: actions/checkout@v3
-
-      - id: install
-        name: Install
-        uses: ./.github/actions/install
-
-      - id: make
-        name: Make
-        run: pipenv run make site
-
   build:
     name: Build release candidate
     runs-on: ubuntu-latest
     needs: [lint-python, test-python, static-type-check]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
```

### Comparing `newshomepages-0.0.8/.github/workflows/performance-report.yml` & `newshomepages-0.0.9/.github/workflows/performance-report.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/reusable-archive-batch-workflow.yml` & `newshomepages-0.0.9/.github/workflows/reusable-archive-batch-workflow.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/reusable-archive-single-site-workflow.yml` & `newshomepages-0.0.9/.github/workflows/reusable-archive-single-site-workflow.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/site.yml` & `newshomepages-0.0.9/.github/workflows/site.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.github/workflows/status-report.yml` & `newshomepages-0.0.9/.github/workflows/status-report.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.gitignore` & `newshomepages-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/.pre-commit-config.yaml` & `newshomepages-0.0.9/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
-#-   repo: https://github.com/pre-commit/pre-commit-hooks
-#    rev: v4.1.0
-#    hooks:
-#    -   id: trailing-whitespace
-#        exclude: newshomepages/extensions/
-#    -   id: end-of-file-fixer
-#        exclude: newshomepages/extensions/
-#    -   id: check-yaml
-#        exclude: newshomepages/extensions/
-#    -   id: check-added-large-files
-#        args: ['--maxkb=100000']
-#    -   id: check-byte-order-marker
-#        exclude: newshomepages/extensions
-#    -   id: check-case-conflict
-#        exclude: newshomepages/extensions/
-#    -   id: check-json
-#        exclude: newshomepages/extensions/
-#    -   id: mixed-line-ending
-#        exclude: newshomepages/extensions/
+-   repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.1.0
+    hooks:
+    -   id: trailing-whitespace
+        exclude: newshomepages/extensions/
+    -   id: end-of-file-fixer
+        exclude: newshomepages/extensions/
+    -   id: check-yaml
+        exclude: newshomepages/extensions/
+    -   id: check-added-large-files
+        args: ['--maxkb=10000']
+    -   id: check-byte-order-marker
+        exclude: newshomepages/extensions
+    -   id: check-case-conflict
+        exclude: newshomepages/extensions/
+    -   id: check-json
+        exclude: newshomepages/extensions/
+    -   id: mixed-line-ending
+        exclude: newshomepages/extensions/
 
 -   repo: https://github.com/psf/black
     rev: 22.3.0
     hooks:
     -   id: black
         exclude: newshomepages/extensions/
```

### Comparing `newshomepages-0.0.8/CODE_OF_CONDUCT.md` & `newshomepages-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/LICENSE` & `newshomepages-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/Makefile` & `newshomepages-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/PKG-INFO` & `newshomepages-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: newshomepages
-Version: 0.0.8
-Summary: A template for open-source Python software repositories
+Version: 0.0.9
+Summary: An open-source archive that gathers, saves, shares and analyzes news homepages
 Home-page: https://homepages.news
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: GPLv3
 Project-URL: Maintainer, https://palewi.re/who-is-ben-welsh/
 Project-URL: Source, https://github.com/palewire/news-homepages
 Project-URL: Tracker, https://github.com/palewire/news-homepages/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: News/Diary
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 An open-source archive that gathers, saves, shares and analyzes news homepages
 
 ## Links
```

### Comparing `newshomepages-0.0.8/Pipfile` & `newshomepages-0.0.9/Pipfile`

 * *Files 12% similar despite different names*

```diff
@@ -52,10 +52,11 @@
 sphinx-click = "*"
 types-retry = "*"
 storysniffer = "*"
 ipywidgets = "*"
 setuptools-scm = "*"
 twine = "*"
 xlwt = "*"
+pytest-env = "*"
 
 [requires]
 python_version = "3.9"
```

### Comparing `newshomepages-0.0.8/Pipfile.lock` & `newshomepages-0.0.9/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9841731266149871%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'80811e5eb74a7286b885468c2dcf3d464a1f880e9a42be0409564f525f163df8'}}",*

 * * "'default'": "{'exceptiongroup': {'hashes': "*

 * *              "['sha256:542adf9dea4055530d6e1279602fa5cb11dab2395fa650b8674eaec35fc4a828', "*

 * *              "'sha256:bd14967b79cd9bdb54d97323216f8fdf533e278df937aa2a90089e7d6e06e5ec'], "*

 * *              "'version': '==1.0.4'}, 'jupyter-server': {'hashes': "*

 * *              "['sha256:69cb954ef02c0ba1837787e34e4a1240c93c8eb590662fae1840778861957660',  […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4f7c06f697498c88b3f8b28da97471ce21da51723f483b233c806091ff944f09"
+            "sha256": "80811e5eb74a7286b885468c2dcf3d464a1f880e9a42be0409564f525f163df8"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -527,19 +527,19 @@
                 "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.4"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:4d6c0aa6dd825810941c792f53d7b8d71da26f5e5f84f20f9508e8f2d33b140a",
-                "sha256:73866f7f842ede6cb1daa42c4af078e2035e5f7607f0e2c762cc51bb31bbe7b2"
+                "sha256:542adf9dea4055530d6e1279602fa5cb11dab2395fa650b8674eaec35fc4a828",
+                "sha256:bd14967b79cd9bdb54d97323216f8fdf533e278df937aa2a90089e7d6e06e5ec"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.0.1"
+            "version": "==1.0.4"
         },
         "executing": {
             "hashes": [
                 "sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc",
                 "sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107"
             ],
             "version": "==1.2.0"
@@ -766,19 +766,19 @@
                 "sha256:6da1fae48190da8551e1b5dbbb19d51d00b079d59a073c7030407ecaf96dbb1e"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==5.0.0"
         },
         "jupyter-server": {
             "hashes": [
-                "sha256:4bdcde2aa576b05da5cf89f33b7d97adcaea5cad4f5863a0db09dcc9eecd66bf",
-                "sha256:cee48d9d96cecd0f94b7cb41ecd4f0ab05b01643769f61c5d397b7873bc9a1e2"
+                "sha256:69cb954ef02c0ba1837787e34e4a1240c93c8eb590662fae1840778861957660",
+                "sha256:c01d0e84c22a14dd6b0e7d8ce4105b08a3426b46582668e28046a64c07311a4f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.23.1"
+            "version": "==1.23.2"
         },
         "jupyterlab": {
             "hashes": [
                 "sha256:e02556c8ea1b386963c4b464e4618aee153c5416b07ab481425c817a033323a2",
                 "sha256:f433059fe0e12d75ea90a81a0b6721113bb132857e3ec2197780b6fe84cbcbde"
             ],
             "index": "pypi",
@@ -790,19 +790,19 @@
                 "sha256:7405d7fde60819d905a9fa8ce89e4cd830e318cdad22a0030f7a901da705585d"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.2.2"
         },
         "jupyterlab-server": {
             "hashes": [
-                "sha256:07007a3a0a30bfc6424b28b76df8d67386cc2d5f9f42886773b1b3c473cb9a3f",
-                "sha256:7ad1a37a716f6d10e90185c636c122d55a58ef3141ae50f9d0601d3ccf54d43e"
+                "sha256:635a0b176a901f19351c02221a124e59317c476f511200409b7d867e8b2905c3",
+                "sha256:d18eb623428b4ee732c2258afaa365eedd70f38b609981ea040027914df32bc6"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.16.2"
+            "version": "==2.16.3"
         },
         "langcodes": {
             "hashes": [
                 "sha256:4d89fc9acb6e9c8fdef70bcdf376113a3db09b67285d9e1d534de6d8818e7e69",
                 "sha256:794d07d5a28781231ac335a1561b8442f8648ca07cd518310aeb45d6f0807ef6"
             ],
             "markers": "python_version >= '3.6'",
@@ -982,19 +982,19 @@
                 "sha256:a1d844efd6da9bc39d2209bf996dbd8e07bf0f36b796edfabaa8f8a9ab77c3aa"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.7.0"
         },
         "nbconvert": {
             "hashes": [
-                "sha256:7bee39e41835642f84599c2841ea53f21f4099257102c07c09347202c3ef732a",
-                "sha256:ed6eb42c2700a1aa5253db25db932db789e3a1ee01e1adf004bfed13c56bff50"
+                "sha256:3e90e108bb5637b5b8a1422af1156af1368b39dd25369ff7faa7dfdcdef18f81",
+                "sha256:8fdc44fd7d9424db7fdc6e1e834a02f6b8620ffb653767388be2f9eb16f84184"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.4"
+            "version": "==7.2.5"
         },
         "nbformat": {
             "hashes": [
                 "sha256:1b05ec2c552c2f1adc745f4eddce1eac8ca9ffd59bb9fd859e827eaa031319f9",
                 "sha256:1d4760c15c1a04269ef5caf375be8b98dd2f696e5eb9e603ec2bf091f9b0d3f3"
             ],
             "markers": "python_version >= '3.7'",
@@ -1137,19 +1137,19 @@
                 "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.8.3"
         },
         "pathy": {
             "hashes": [
-                "sha256:3178215bdadf3741107d987020be0fb5b59888f60f96de43cce5fe45d9d4b64a",
-                "sha256:a7aa9794fade161bb4c28a33c5bc2c6bf41f61ec5eee51cfa8914f0a433447e1"
+                "sha256:7da78fc4b6188d5e62c7aeea1676e6875b9e88e70bbe899c466e4cdb450fd4f1",
+                "sha256:899e88fe848b58d9823423bd6f94fbc76f48af29245925b4736aaf6756be4533"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==0.6.2"
+            "version": "==0.8.1"
         },
         "pexpect": {
             "hashes": [
                 "sha256:0b48a55dcb3c05f3329815901ea4fc1537514d6ba867a152b581d69ae3710937",
                 "sha256:fc65a43959d153d0114afe13997d439c22823a27cefceb5ff35c2178c6784c0c"
             ],
             "markers": "sys_platform != 'win32'",
@@ -1227,19 +1227,19 @@
                 "sha256:f1ff2ee69f10f13a9596480335f406dd1f70c3650349e2be67ca3139280cade0"
             ],
             "index": "pypi",
             "version": "==9.3.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0cb405749187a194f444c25c82ef7225232f11564721eabffc6ec70df83b11cb",
-                "sha256:6e52c21afff35cb659c6e52d8b4d61b9bd544557180440538f255d9382c8cbe0"
+                "sha256:1006647646d80f16130f052404c6b901e80ee4ed6bef6792e1f238a8969106f7",
+                "sha256:af0276409f9a02373d540bf8480021a048711d572745aef4b7842dad245eba10"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.3"
+            "version": "==2.5.4"
         },
         "playwright": {
             "hashes": [
                 "sha256:217b2f623527ded15d602ccca5138395a1677c67399c4494844d5341420d34e0",
                 "sha256:78ddf51d0c08d94edb6d2ddf7b262f0d87a1c0ab5e121bfefa1945214c308f95",
                 "sha256:9506d582e1a36aa19b06f5b5f8ae154265ec2fc5039217cfe8dfd66edb1a7563",
                 "sha256:a36dfaf9be0228985b7b001887f66dc61e8300970c0602ae9d5b191da510a982",
@@ -1480,19 +1480,19 @@
                 "sha256:9c45335c81aa288a28e45e66484306e340777adac01e6cb2ee84c9909ffa3f18"
             ],
             "index": "pypi",
             "version": "==2022.9.17"
         },
         "python-slugify": {
             "hashes": [
-                "sha256:272d106cb31ab99b3496ba085e3fea0e9e76dcde967b5e9992500d1f785ce4e1",
-                "sha256:7b2c274c308b62f4269a9ba701aa69a797e9bca41aeee5b3a9e79e36b6656927"
+                "sha256:003aee64f9fd955d111549f96c4b58a3f40b9319383c70fad6277a4974bbf570",
+                "sha256:7a0f21a39fa6c1c4bf2e5984c9b9ae944483fd10b54804cb0e23a3ccd4954f0b"
             ],
             "index": "pypi",
-            "version": "==6.1.2"
+            "version": "==7.0.0"
         },
         "python-telegram-bot": {
             "hashes": [
                 "sha256:79abc66355af2310bbaaf7f41746230b996434e287f21f27070c92978dc0964f",
                 "sha256:e9391d43eb1123de2677a9d24ea878a9d5327d65b2419afba653f476d26aecc3"
             ],
             "index": "pypi",
@@ -1795,15 +1795,15 @@
             "version": "==1.16.0"
         },
         "smart-open": {
             "hashes": [
                 "sha256:71d14489da58b60ce12fc3ecb823facc59a8b23cd1b58edb97175640350d3a62",
                 "sha256:75abf758717a92a8f53aa96953f0c245c8cedf8e1e4184903db3659b419d4c17"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
+            "markers": "python_version >= '3.6' and python_full_version < '4.0.0'",
             "version": "==5.2.1"
         },
         "sniffio": {
             "hashes": [
                 "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
                 "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
             ],
@@ -1823,45 +1823,45 @@
                 "sha256:fc53893b3da2c33de295667a0e19f078c14bf86544af307354de5fcf12a3f30d"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.3.2.post1"
         },
         "spacy": {
             "hashes": [
-                "sha256:0286e243f748956e7336b6d59ac23319ef9c5ea0a5d772c2fd96ab77f889d09b",
-                "sha256:1cefddd9cb8295c86410485cb4d783dae7cf3f860019402633cc93a2ee159759",
-                "sha256:1dd805ac6af9e796ff46df3d5582a062e228637c57ab38e0e4c48c161604473b",
-                "sha256:3216737a0e53382b13324f691eedbf5f86bd05b6f405af7049c467eda07d4c69",
-                "sha256:3563df6793cc094202ef8b56ab60e2eaf9cc95a55b70c1e5da36c35b3efd4695",
-                "sha256:38c6f77971c4f509ad40176484935cab30a64ea0599233253885e6412294ccd4",
-                "sha256:3b8df4d67d6166b94568c3ec7ab9624dbd7d41aa96ceecf063e1e74a8e0e44ea",
-                "sha256:469628cfd2760a15188fb9ca5419ebdef3f533ba2897486089d84c8173a76168",
-                "sha256:61fd0e7e526494b5019e21fae352f3cee26d2fbeea8db9897325e05b0376f96b",
-                "sha256:64c8d41f11c09b86140efed8a2e3e4d913b81ee8315bcab166f4409fbc461eed",
-                "sha256:681aa6532baa62a0385dfcc58ac53017c2614cd63a6afafe9c881ef9994a1c58",
-                "sha256:6aab72be4bd5df5f55dc87a8711df0e5e24bdaa4e4a5f321518fa6ff49d7cb61",
-                "sha256:956afb7ced04a29faff826d479ed4eec6447906104c985ead883fa83f16920b9",
-                "sha256:9623b97c880ad0a7a81b8b9b0b88e7d1fef974950c4e7bd56ea58d62accd86b3",
-                "sha256:9ad2f094389669df481c5fa16961b1749ee7c14bdd07a60fe5ed49d8641b14cf",
-                "sha256:9bd8bd225233aa8e28ca7dfe79d3a148f11a61164444bddc77f224f66f3e9003",
-                "sha256:9dc21decf096726784a905ba3d4d366915b938e1b67bfd98e8d8f0201ddc207d",
-                "sha256:a0a07345acce60c78cf5a8511764906e20a805985389376cb4ee80e8a7b62755",
-                "sha256:a81f9d9cdb39a33125291bc753b54448c883ff1952ffb73a3a8a4ad6c1e51ef5",
-                "sha256:b17355df0ca832a3e663a2c618a591fb4fa9bf0c0c252d64aacc11ddd71c3fc8",
-                "sha256:b27c2c6ca7b1818667a334bb9efd78d39ce6920b2387812b81955b1a8cfbfbe9",
-                "sha256:ca14c622f7c569a87f6e315a09bacc44753091e3ba6362ba525e88a330532b7e",
-                "sha256:d334acfab6786cb0d9976e5761ffadd2359c508c068f1c2794f9aab86be9be9d",
-                "sha256:d50f786114a45defd364adc79468964c5b07734b76e7ae8360426277bc6b8008",
-                "sha256:dbf245a7573cd035c8d58e9017ed0aa0b10e5f70a4c711992905cc68fcd900be",
-                "sha256:efec86dc4162b7ff0a08e539dce10c4454c317bfbf4d6ed7cceaea20cb3c8c62",
-                "sha256:fb3b8ec1741d16c9ae2da3f4ad629c88569cb1219e9622812bb1d7fdb9ef003f",
-                "sha256:ff4daa912df17d639315a3438813e84d51bf2527bbd0d6a56c9e3c9cbcfb0344"
+                "sha256:0cdc23a48e6543402b4c56ebf2d36246001175c29fd56d3081efcec684651abc",
+                "sha256:22698cf5175e2b697e82699fcccee3092b42137a57d352df208d71657fd693bb",
+                "sha256:2ddba486c4c981abe6f1e3fd72648dc8811966e5f0e05808f9c9fab155c388d7",
+                "sha256:2ea41f9de30435456235c4182d8bc2eb54a0a64719856e66e780350bb4c8cfbe",
+                "sha256:36a9a506029842795099fd97ad95f0da2845c319020fcc7164cbf33650726f83",
+                "sha256:3b3e629c889cac9656151286ec1232c6a948ce0d44a39f1ef5e60fed4f183a10",
+                "sha256:3c87117dd335fba44d1c0d77602f0763c3addf4e7ef9bdbe9a495466c3484c69",
+                "sha256:3ce3938720f48eaeeb360a7f623f15a0d9efd1a688d5d740e3d4cdcd6f6da8a3",
+                "sha256:455c2fbd1de24b6fe34fa121d87525134d7498f9f458ebc8274d7940b473999e",
+                "sha256:462e141f514d78cff85685b5b12eb8cadac0bad2f7820149cbe18d03ccb2e59c",
+                "sha256:5ab293eb1423fa05c7ee71b2fedda57c2b4a4ca8dc054ce678809457287b01dc",
+                "sha256:5c0d65f39184f522b4e67b965a42d121a3b2d799362682fe8847b64b0ce5bc7c",
+                "sha256:676ab9ab2cf94ba48caa306f185a166e85bd35b388ec24512c8ba7dfcbc7517e",
+                "sha256:6ad6bf5e4e7f0bc2ef94b7ff6fe59abd766f74c192bca2f17430a3b3cd5bda5a",
+                "sha256:7115da36369b3c537caf2fe08e0b45528bd091c7f56ba3580af1e6fdfa9b1081",
+                "sha256:9277cd0fcb96ee5dd885f7e96c639f21afd96198d61ca32100446afbff4dfbef",
+                "sha256:a36bd06a5a147350e5f5f6903c4777296c37b18199251bb41056c3a73aa4494f",
+                "sha256:a7b97ec21ed773edb2479ae5d6c7686b8034f418df6bccd9218f5c3c2b7cf888",
+                "sha256:afaf6e716cbac4a0fbfa9e9bf95decff223936597ddd03ea869118a7576aa1b1",
+                "sha256:bb6d0f185126decc8392cde7d28eb6e85ba4bca15424713288cccc49c2a3c52b",
+                "sha256:bdafcd0823ca804c39d0bed9e677eb7d0235b1259563d0fd4d3a201c71108af8",
+                "sha256:c966d25b3f3e49f5de08546b3638928f49678c365cbbebd0eec28f74e0adb539",
+                "sha256:d1c85279fbb6b75d7fb8d7c59c2b734502e51271cad90926e8df1d21b67da5aa",
+                "sha256:d211c2b8894354bf8d961af9a9dcab38f764e1dcddd7b80760e438fcd4c9fe43",
+                "sha256:ded11aa8966236aab145b4d2d024b3eb61ac50078362d77d9ed7d8c240ef0f4a",
+                "sha256:e546b314f619502ae03e5eb9a0cfd09ca7a9db265bcdd8a3af83cfb0f1432e55",
+                "sha256:e6b871de8857a6820140358db3943180fdbe03d44ed792155cee6cb95f4ac4ea",
+                "sha256:f6644c678bd7af567c6ce679f71d64119282e7d6f1a6f787162a91be3ea39333"
             ],
             "index": "pypi",
-            "version": "==3.4.2"
+            "version": "==3.4.3"
         },
         "spacy-legacy": {
             "hashes": [
                 "sha256:16104595d8ab1b7267f817a449ad1f986eb1f2a2edf1050748f08739a479679a",
                 "sha256:8526a54d178dee9b7f218d43e5c21362c59056c5da23380b319b56043e9211f3"
             ],
             "markers": "python_version >= '3.6'",
@@ -1914,18 +1914,18 @@
                 "sha256:facab907801fbcb0e54b3532e04bc6a0709184d68004ef3a129e8c7e3ca63d82"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.4.5"
         },
         "stack-data": {
             "hashes": [
-                "sha256:8e515439f818efaa251036af72d89e4026e2b03993f3453c000b200fb4f2d6aa",
-                "sha256:b92d206ef355a367d14316b786ab41cb99eb453a21f2cb216a4204625ff7bc07"
+                "sha256:6c9a10eb5f342415fe085db551d673955611afb821551f554d91772415464315",
+                "sha256:960cb054d6a1b2fdd9cbd529e365b3c163e8dabf1272e02cfe36b58403cff5c6"
             ],
-            "version": "==0.6.0"
+            "version": "==0.6.1"
         },
         "storysniffer": {
             "hashes": [
                 "sha256:930cd8d15aab9b3c55bfc14db8f12b6f045e4fe686e0d5dc934bdb56ea9555b9",
                 "sha256:a5f1273bfb881178be89913bca5c3e71600585dc8b3ea0de7127546c76dd57f4"
             ],
             "index": "pypi",
@@ -2097,19 +2097,19 @@
                 "sha256:a3d34de8fac26023eee701ed1e7bf4da9a8326b61a62934ec9e53b64970fd8fe"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==0.9.2"
         },
         "typer": {
             "hashes": [
-                "sha256:023bae00d1baf358a6cc7cea45851639360bb716de687b42b0a4641cd99173f1",
-                "sha256:b8261c6c0152dd73478b5ba96ba677e5d6948c715c310f7c91079f311f62ec03"
+                "sha256:b5e704f4e48ec263de1c0b3a2387cd405a13767d2f907f44c1a08cbad96f606d",
+                "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==0.4.2"
+            "version": "==0.7.0"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
                 "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
             ],
             "markers": "python_version >= '3.7'",
@@ -2132,15 +2132,15 @@
             "version": "==4.2"
         },
         "urllib3": {
             "hashes": [
                 "sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e",
                 "sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4.0'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_full_version < '4.0.0'",
             "version": "==1.26.12"
         },
         "urllib3-secure-extra": {
             "hashes": [
                 "sha256:ee9409cbfeb4b8609047be4c32fb4317870c602767e53fd8a41005ebe6a41dff",
                 "sha256:f7adcb108b4d12a4b26b99eb60e265d087f435052a76aefa396b6ee85e9a6ef9"
             ],
@@ -2565,19 +2565,19 @@
                 "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.4"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:4d6c0aa6dd825810941c792f53d7b8d71da26f5e5f84f20f9508e8f2d33b140a",
-                "sha256:73866f7f842ede6cb1daa42c4af078e2035e5f7607f0e2c762cc51bb31bbe7b2"
+                "sha256:542adf9dea4055530d6e1279602fa5cb11dab2395fa650b8674eaec35fc4a828",
+                "sha256:bd14967b79cd9bdb54d97323216f8fdf533e278df937aa2a90089e7d6e06e5ec"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.0.1"
+            "version": "==1.0.4"
         },
         "executing": {
             "hashes": [
                 "sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc",
                 "sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107"
             ],
             "version": "==1.2.0"
@@ -2612,19 +2612,19 @@
                 "sha256:9fe7c6a306064af8e62a055c2f61e9eb1da55f84bb39caef2b84ce53708ac34b"
             ],
             "index": "pypi",
             "version": "==1.6.0"
         },
         "identify": {
             "hashes": [
-                "sha256:48b7925fe122720088aeb7a6c34f17b27e706b72c61070f27fe3789094233440",
-                "sha256:7a214a10313b9489a0d61467db2856ae8d0b8306fc923e03a9effa53d8aedc58"
+                "sha256:906036344ca769539610436e40a684e170c3648b552194980bb7b617a8daeb9f",
+                "sha256:a390fb696e164dbddb047a0db26e57972ae52fbd037ae68797e5ae2f4492485d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.8"
+            "version": "==2.5.9"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -2847,47 +2847,47 @@
                 "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.0.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:0680389c34284287fe00e82fc8bccdea9aff318f7e7d55b90d967a13a9606013",
-                "sha256:1767830da2d1afa4e62b684647af0ff79b401f004d7fa08bc5b0ce2d45bcd5ec",
-                "sha256:1ee5f99817ee70254e7eb5cf97c1b11dda29c6893d846c8b07bce449184e9466",
-                "sha256:262c543ef24deb10470a3c1c254bb986714e2b6b1a67d66daf836a548a9f316c",
-                "sha256:269f0dfb6463b8780333310ff4b5134425157ef0d2b1d614015adaf6d6a7eabd",
-                "sha256:2a3150d409609a775c8cb65dbe305c4edd7fe576c22ea79d77d1454acd9aeda8",
-                "sha256:2b6f85c2ad378e3224e017904a051b26660087b3b76490d533b7344f1546d3ff",
-                "sha256:3227f14fe943524f5794679156488f18bf8d34bfecd4623cf76bc55958d229c5",
-                "sha256:3ff201a0c6d3ea029d73b1648943387d75aa052491365b101f6edd5570d018ea",
-                "sha256:46897755f944176fbc504178422a5a2875bbf3f7436727374724842c0987b5af",
-                "sha256:47a9955214615108c3480a500cfda8513a0b1cd3c09a1ed42764ca0dd7b931dd",
-                "sha256:49082382f571c3186ce9ea0bd627cb1345d4da8d44a8377870f4442401f0a706",
-                "sha256:4a8a6c10f4c63fbf6ad6c03eba22c9331b3946a4cec97f008e9ffb4d3b31e8e2",
-                "sha256:6826d9c4d85bbf6d68cb279b561de6a4d8d778ca8e9ab2d00ee768ab501a9852",
-                "sha256:72382cb609142dba3f04140d016c94b4092bc7b4d98ca718740dc989e5271b8d",
-                "sha256:7da0005e47975287a92b43276e460ac1831af3d23032c34e67d003388a0ce8d0",
-                "sha256:8798c8ed83aa809f053abff08664bdca056038f5a02af3660de00b7290b64c47",
-                "sha256:8f1940325a8ed460ba03d19ab83742260fa9534804c317224e5d4e5aa588e2d6",
-                "sha256:8f694d6d09a460b117dccb6857dda269188e3437c880d7b60fa0014fa872d1e9",
-                "sha256:9b8f4a8213b1fd4b751e26b59ae0e0c12896568d7e805861035c7a15ed6dc9eb",
-                "sha256:9d851c09b981a65d9d283a8ccb5b1d0b698e580493416a10942ef1a04b19fd37",
-                "sha256:aaf1be63e0207d7d17be942dcf9a6b641745581fe6c64df9a38deb562a7dbafa",
-                "sha256:aba38e3dd66bdbafbbfe9c6e79637841928ea4c79b32e334099463c17b0d90ef",
-                "sha256:b08541a06eed35b543ae1a6b301590eb61826a1eb099417676ddc5a42aa151c5",
-                "sha256:be88d665e76b452c26fb2bdc3d54555c01226fba062b004ede780b190a50f9db",
-                "sha256:c76c769c46a1e6062a84837badcb2a7b0cdb153d68601a61f60739c37d41cc74",
-                "sha256:cc6019808580565040cd2a561b593d7c3c646badd7e580e07d875eb1bf35c695",
-                "sha256:cd2dd3730ba894ec2a2082cc703fbf3e95a08479f7be84912e3131fc68809d46",
-                "sha256:d555aa7f44cecb7ea3c0ac69d58b1a5afb92caa017285a8e9c4efbf0518b61b4",
-                "sha256:d847dd23540e2912d9667602271e5ebf25e5788e7da46da5ffd98e7872616e8e"
+                "sha256:0714258640194d75677e86c786e80ccf294972cc76885d3ebbb560f11db0003d",
+                "sha256:0c8f3be99e8a8bd403caa8c03be619544bc2c77a7093685dcf308c6b109426c6",
+                "sha256:0cca5adf694af539aeaa6ac633a7afe9bbd760df9d31be55ab780b77ab5ae8bf",
+                "sha256:1c8cd4fb70e8584ca1ed5805cbc7c017a3d1a29fb450621089ffed3e99d1857f",
+                "sha256:1f7d1a520373e2272b10796c3ff721ea1a0712288cafaa95931e66aa15798813",
+                "sha256:209ee89fbb0deed518605edddd234af80506aec932ad28d73c08f1400ef80a33",
+                "sha256:26efb2fcc6b67e4d5a55561f39176821d2adf88f2745ddc72751b7890f3194ad",
+                "sha256:37bd02ebf9d10e05b00d71302d2c2e6ca333e6c2a8584a98c00e038db8121f05",
+                "sha256:3a700330b567114b673cf8ee7388e949f843b356a73b5ab22dd7cff4742a5297",
+                "sha256:3c0165ba8f354a6d9881809ef29f1a9318a236a6d81c690094c5df32107bde06",
+                "sha256:3d80e36b7d7a9259b740be6d8d906221789b0d836201af4234093cae89ced0cd",
+                "sha256:4175593dc25d9da12f7de8de873a33f9b2b8bdb4e827a7cae952e5b1a342e243",
+                "sha256:4307270436fd7694b41f913eb09210faff27ea4979ecbcd849e57d2da2f65305",
+                "sha256:5e80e758243b97b618cdf22004beb09e8a2de1af481382e4d84bc52152d1c476",
+                "sha256:641411733b127c3e0dab94c45af15fea99e4468f99ac88b39efb1ad677da5711",
+                "sha256:652b651d42f155033a1967739788c436491b577b6a44e4c39fb340d0ee7f0d70",
+                "sha256:6d7464bac72a85cb3491c7e92b5b62f3dcccb8af26826257760a552a5e244aa5",
+                "sha256:74e259b5c19f70d35fcc1ad3d56499065c601dfe94ff67ae48b85596b9ec1461",
+                "sha256:7d17e0a9707d0772f4a7b878f04b4fd11f6f5bcb9b3813975a9b13c9332153ab",
+                "sha256:901c2c269c616e6cb0998b33d4adbb4a6af0ac4ce5cd078afd7bc95830e62c1c",
+                "sha256:98e781cd35c0acf33eb0295e8b9c55cdbef64fcb35f6d3aa2186f289bed6e80d",
+                "sha256:a12c56bf73cdab116df96e4ff39610b92a348cc99a1307e1da3c3768bbb5b135",
+                "sha256:ac6e503823143464538efda0e8e356d871557ef60ccd38f8824a4257acc18d93",
+                "sha256:b8472f736a5bfb159a5e36740847808f6f5b659960115ff29c7cecec1741c648",
+                "sha256:b86ce2c1866a748c0f6faca5232059f881cda6dda2a893b9a8373353cfe3715a",
+                "sha256:bc9ec663ed6c8f15f4ae9d3c04c989b744436c16d26580eaa760ae9dd5d662eb",
+                "sha256:c9166b3f81a10cdf9b49f2d594b21b31adadb3d5e9db9b834866c3258b695be3",
+                "sha256:d13674f3fb73805ba0c45eb6c0c3053d218aa1f7abead6e446d474529aafc372",
+                "sha256:de32edc9b0a7e67c2775e574cb061a537660e51210fbf6006b0b36ea695ae9bb",
+                "sha256:e62ebaad93be3ad1a828a11e90f0e76f15449371ffeecca4a0a0b9adc99abcef"
             ],
             "index": "pypi",
-            "version": "==0.990"
+            "version": "==0.991"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d",
                 "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"
             ],
             "version": "==0.4.3"
@@ -3020,19 +3020,19 @@
                 "sha256:a84da4318dd86f870a9447a8c98340aa06216bfc6f2b7bdc4b8766984ae1867c"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.8.3"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0cb405749187a194f444c25c82ef7225232f11564721eabffc6ec70df83b11cb",
-                "sha256:6e52c21afff35cb659c6e52d8b4d61b9bd544557180440538f255d9382c8cbe0"
+                "sha256:1006647646d80f16130f052404c6b901e80ee4ed6bef6792e1f238a8969106f7",
+                "sha256:af0276409f9a02373d540bf8480021a048711d572745aef4b7842dad245eba10"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.3"
+            "version": "==2.5.4"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -3147,14 +3147,22 @@
             "hashes": [
                 "sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71",
                 "sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59"
             ],
             "index": "pypi",
             "version": "==7.2.0"
         },
+        "pytest-env": {
+            "hashes": [
+                "sha256:8c0605ae09a5b7e41c20ebcc44f2c906eea9654095b4b0c342b3814bcc3a8492",
+                "sha256:d7b2f5273ec6d1e221757998bc2f50d2474ed7d0b9331b92556011fadc4e9abf"
+            ],
+            "index": "pypi",
+            "version": "==0.8.1"
+        },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
@@ -3511,18 +3519,18 @@
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
         "stack-data": {
             "hashes": [
-                "sha256:8e515439f818efaa251036af72d89e4026e2b03993f3453c000b200fb4f2d6aa",
-                "sha256:b92d206ef355a367d14316b786ab41cb99eb453a21f2cb216a4204625ff7bc07"
+                "sha256:6c9a10eb5f342415fe085db551d673955611afb821551f554d91772415464315",
+                "sha256:960cb054d6a1b2fdd9cbd529e365b3c163e8dabf1272e02cfe36b58403cff5c6"
             ],
-            "version": "==0.6.0"
+            "version": "==0.6.1"
         },
         "storysniffer": {
             "hashes": [
                 "sha256:930cd8d15aab9b3c55bfc14db8f12b6f045e4fe686e0d5dc934bdb56ea9555b9",
                 "sha256:a5f1273bfb881178be89913bca5c3e71600585dc8b3ea0de7127546c76dd57f4"
             ],
             "index": "pypi",
@@ -3621,19 +3629,19 @@
                 "sha256:96b1cf12f7ae611a4a40b6ae8e9570215daff0611828f5fe1f37a16255ab24a0"
             ],
             "index": "pypi",
             "version": "==4.0.1"
         },
         "types-python-slugify": {
             "hashes": [
-                "sha256:556d9b387ef632e588445b9e0edbb0e57e939ab387e53a05ad9c5a6d1321b2a3",
-                "sha256:663de4a7ce61c5448e838ffd2e34748df6631d4588dc0ed9a7c2bf973c0314ed"
+                "sha256:21fd3af49842944acf96f07e320399fac51fdb9c857b7bf1cf2118526e252a22",
+                "sha256:260d08ab291d15fa7ab26b95bfb23eddb422aaeb9b9182d0da46decbf751349e"
             ],
             "index": "pypi",
-            "version": "==6.1.0"
+            "version": "==6.1.0.1"
         },
         "types-pytz": {
             "hashes": [
                 "sha256:bea605ce5d5a5d52a8e1afd7656c9b42476e18a0f888de6be91587355313ddf4",
                 "sha256:d078196374d1277e9f9984d49373ea043cf2c64d5d5c491fbc86c258557bd46f"
             ],
             "index": "pypi",
@@ -3645,58 +3653,58 @@
                 "sha256:6840819871c92deebe6a2067fb800c11b8a063632eb4e3e755914e7ab3604e83"
             ],
             "index": "pypi",
             "version": "==6.0.12.2"
         },
         "types-requests": {
             "hashes": [
-                "sha256:bdb1f9811e53d0642c8347b09137363eb25e1a516819e190da187c29595a1df3",
-                "sha256:d4f342b0df432262e9e326d17638eeae96a5881e78e7a6aae46d33870d73952e"
+                "sha256:091d4a5a33c1b4f20d8b1b952aa8fa27a6e767c44c3cf65e56580df0b05fd8a9",
+                "sha256:a7df37cc6fb6187a84097da951f8e21d335448aa2501a6b0a39cbd1d7ca9ee2a"
             ],
             "index": "pypi",
-            "version": "==2.28.11.4"
+            "version": "==2.28.11.5"
         },
         "types-retry": {
             "hashes": [
                 "sha256:b1087b274680b542c796549e8488898d0b22cd89988ef1016ef56d4367ff4f41",
                 "sha256:c5208407527661c37ee826a81abe8e7560e138c8deeccce61bf3f5441f2085f0"
             ],
             "index": "pypi",
             "version": "==0.9.9"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:1807b87b8ee1ae0226813ba2c52330eff20fb2bf6359b1de24df08eb3090e442",
-                "sha256:a188c24fc61a99658c8c324c8dd7419f5b91a0d89df004e5f576869122c1db55"
+                "sha256:ed6b9e8a8be488796f72306889a06a3fc3cb1aa99af02ab8afb50144d7317e49",
+                "sha256:eec5556428eec862b1ac578fb69aab3877995a99ffec9e5a12cf7fbd0cc9daee"
             ],
-            "version": "==1.26.25.3"
+            "version": "==1.26.25.4"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
                 "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.4.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e",
                 "sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4.0'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_full_version < '4.0.0'",
             "version": "==1.26.12"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:186ca84254abcbde98180fd17092f9628c5fe742273c02724972a1d8a2035108",
-                "sha256:530b850b523c6449406dfba859d6345e48ef19b8439606c5d74d7d3c9e14d76e"
+                "sha256:8691e3ff9387f743e00f6bb20f70121f5e4f596cae754531f2b3b3a1b1ac696e",
+                "sha256:efd66b00386fdb7dbe4822d172303f40cd05e50e01740b19ea42425cbe653e29"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==20.16.6"
+            "version": "==20.16.7"
         },
         "wcwidth": {
             "hashes": [
                 "sha256:beb4802a9cebb9144e99086eff703a642a13d6a0052920003a230f3294bbe784",
                 "sha256:c4d647b99872929fdb7bdcaa4fbe7f01413ed3d98077df798530e5b04f116c83"
             ],
             "version": "==0.2.5"
```

### Comparing `newshomepages-0.0.8/README.md` & `newshomepages-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/accessibility.py` & `newshomepages-0.0.9/newshomepages/accessibility.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/altair_theme.py` & `newshomepages-0.0.9/newshomepages/altair_theme.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/analyze.py` & `newshomepages-0.0.9/newshomepages/analyze.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/batch.py` & `newshomepages-0.0.9/newshomepages/batch.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/discorder.py` & `newshomepages-0.0.9/newshomepages/discorder.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ar/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ar/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/be/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/be/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/bg/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/bg/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ca/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ca/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/cs/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/cs/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/da/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/da/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/de/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/de/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/el/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/el/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/en/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/es/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/es/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/es_419/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/es_419/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/et/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/et/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fa/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fa/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fi/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/fr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/fr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/he/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/he/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hi/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hu/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hu/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/hy/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/hy/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/id/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/id/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/it/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/it/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ja/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ja/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ko/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ko/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/lt/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/lt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ms/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ms/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/nb/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/nb/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/nl/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/nl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pl/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pt_BR/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pt_BR/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/pt_PT/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/pt_PT/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ro/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ro/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/ru/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sk/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sl/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/sv/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/sv/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/th/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/th/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/tr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/tr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/uk/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/uk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/vi/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/vi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/zh_CN/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/zh_CN/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/_locales/zh_TW/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/_locales/zh_TW/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/alert-popup.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/alert-popup.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/c3.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/c3.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/custom.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/custom.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/dark.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/dark.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/layout.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/layout.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/log.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/log.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/css/style.css` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-off-19.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-off-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-off-38.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-off-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-on-19.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-on-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/b13-on-38.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/b13-on-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/gray-19.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/gray-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/gray-38.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/gray-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-128.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-128.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-16.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-16.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-19.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/icons/green-38.png` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/icons/green-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/alert.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/alert.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/app-store.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/app-store.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/arrow-down.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/avatar.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/avatar.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/checked.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/checked.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/chrome.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/chrome.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/cross.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/cross.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/dropbox.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/dropbox.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/favicon.ico` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/filters.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/filters.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/google-play.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/google-play.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/hero-green.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/hero-green.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/hero-red.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/hero-red.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo-dark.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo-shield.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo-shield.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/logo_adguard.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/logo_adguard.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/reload-ico.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/reload-ico.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/tick.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/tick.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/images/toggler-bg.svg` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/images/toggler-bg.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/js/preload-theme.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/js/preload-theme.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml` & `newshomepages-0.0.9/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/content-script/subscribe.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/content-script/subscribe.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_1.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_1.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_10.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_10.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_11.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_11.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_12.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_12.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_13.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_13.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_14.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_14.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_15.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_15.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_16.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_16.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_17.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_17.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_2.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_2.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_224.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_224.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_3.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_3.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_4.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_4.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_5.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_5.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_6.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_6.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_7.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_7.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_8.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_8.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_9.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_9.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_1.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_1.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_10.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_10.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_11.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_11.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_12.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_12.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_13.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_13.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_14.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_14.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_15.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_15.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_16.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_16.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_17.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_17.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_2.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_2.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_224.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_224.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_3.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_3.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_4.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_4.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_5.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_5.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_6.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_6.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_7.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_7.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_8.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_8.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filter_mobile_9.txt` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filter_mobile_9.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filters.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filters.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/filters_i18n.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/filters_i18n.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/filters/local_script_rules.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/filters/local_script_rules.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/manifest.json` & `newshomepages-0.0.9/newshomepages/extensions/adguard/manifest.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/ad-blocked.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/ad-blocked.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/assistant.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/assistant.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/background.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/background.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/content-script-end.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/content-script-end.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/content-script-start.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/content-script-start.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/devtools.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/devtools.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filter-download.html` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filter-download.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filter-download.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filter-download.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/filtering-log.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/filtering-log.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/options.html` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/options.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/options.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/options.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/popup.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/popup.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/safebrowsing.html` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/safebrowsing.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/safebrowsing.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/safebrowsing.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/pages/thankyou.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/pages/thankyou.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/runtime.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/runtime.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/shared/editor.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/shared/editor.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/mobx.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/mobx.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/react.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/react.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/vendors/xstate.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/vendors/xstate.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js` & `newshomepages-0.0.9/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/be/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/be/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/cs/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/cs/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/da/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/da/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/de/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/de/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/en/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/es/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/es/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fi/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/fr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/fr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/he/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/he/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/hu/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/hu/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/id/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/id/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/it/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/it/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ja/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ja/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ko/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ko/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/lt/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/lt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/nl/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/nl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/no/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/no/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pl/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pt/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ro/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ro/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/ru/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sk/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sl/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/sr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/sr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/tr/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/tr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/uk/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/uk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/vi/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/vi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/zh/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/zh/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_installed.png` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_installed.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/assets/images/extra_logo.png` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/assets/images/extra_logo.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/content-script.js` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/content-script.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/manifest.json` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/manifest.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/options.js` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/options.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/popup.html` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/popup.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/adguardextra/userscript.js` & `newshomepages-0.0.9/newshomepages/extensions/adguardextra/userscript.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file-bootstrap.js` & `newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file-bootstrap.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file-frames.js` & `newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file-frames.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file-hooks-frames.js` & `newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file-hooks-frames.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extensions/singlefile/javascript/single-file.js` & `newshomepages-0.0.9/newshomepages/extensions/singlefile/javascript/single-file.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/extract.py` & `newshomepages-0.0.9/newshomepages/extract.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/html.py` & `newshomepages-0.0.9/newshomepages/html.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/hyperlinks.py` & `newshomepages-0.0.9/newshomepages/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/mosaic.py` & `newshomepages-0.0.9/newshomepages/mosaic.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/rss.py` & `newshomepages-0.0.9/newshomepages/rss.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/screenshot.py` & `newshomepages-0.0.9/newshomepages/screenshot.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/site.py` & `newshomepages-0.0.9/newshomepages/site.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/slack.py` & `newshomepages-0.0.9/newshomepages/slack.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/sources/bundles.csv` & `newshomepages-0.0.9/newshomepages/sources/bundles.csv`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/sources/javascript/news_letter.js` & `newshomepages-0.0.9/newshomepages/sources/javascript/news_letter.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/sources/sites.csv` & `newshomepages-0.0.9/newshomepages/sources/sites.csv`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/telegrammer.py` & `newshomepages-0.0.9/newshomepages/telegrammer.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/tweet.py` & `newshomepages-0.0.9/newshomepages/tweet.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/utils.py` & `newshomepages-0.0.9/newshomepages/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages/wayback.py` & `newshomepages-0.0.9/newshomepages/wayback.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/newshomepages.egg-info/PKG-INFO` & `newshomepages-0.0.9/newshomepages.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: newshomepages
-Version: 0.0.8
-Summary: A template for open-source Python software repositories
+Version: 0.0.9
+Summary: An open-source archive that gathers, saves, shares and analyzes news homepages
 Home-page: https://homepages.news
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: GPLv3
 Project-URL: Maintainer, https://palewi.re/who-is-ben-welsh/
 Project-URL: Source, https://github.com/palewire/news-homepages
 Project-URL: Tracker, https://github.com/palewire/news-homepages/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: News/Diary
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 An open-source archive that gathers, saves, shares and analyzes news homepages
 
 ## Links
```

### Comparing `newshomepages-0.0.8/newshomepages.egg-info/SOURCES.txt` & `newshomepages-0.0.9/newshomepages.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+.flake8
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 Pipfile
 Pipfile.lock
 README.md
 SECURITY.md
-setup.cfg
+mypy.ini
+pytest.ini
 setup.py
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/add-a-site.md
 .github/ISSUE_TEMPLATE/report-a-broken-site.md
 .github/actions/accessibility/action.yml
 .github/actions/archive/action.yml
@@ -27,40 +29,35 @@
 .github/actions/slack/action.yml
 .github/actions/telegram/action.yml
 .github/actions/tweet/action.yml
 .github/actions/upload/action.yml
 .github/actions/wayback/action.yml
 .github/workflows/accessibility-report.yml
 .github/workflows/archive-ajc.yml
-.github/workflows/archive-all-batch-1.yml
 .github/workflows/archive-all-batch-10.yml
 .github/workflows/archive-all-batch-2.yml
 .github/workflows/archive-all-batch-3.yml
 .github/workflows/archive-all-batch-4.yml
 .github/workflows/archive-all-batch-5.yml
 .github/workflows/archive-all-batch-6.yml
 .github/workflows/archive-all-batch-7.yml
 .github/workflows/archive-all-batch-8.yml
 .github/workflows/archive-all-batch-9.yml
 .github/workflows/archive-baltimoresun.yml
 .github/workflows/archive-bundle.yml
-.github/workflows/archive-country.yml
 .github/workflows/archive-globeandmail.yml
 .github/workflows/archive-latimes.yaml
 .github/workflows/archive-single-site.yml
 .github/workflows/bln.yml
 .github/workflows/continuous-deployment.yml
 .github/workflows/performance-report.yml
 .github/workflows/reusable-archive-batch-workflow.yml
-.github/workflows/reusable-archive-bundle-workflow.yml
-.github/workflows/reusable-archive-country-workflow.yml
 .github/workflows/reusable-archive-single-site-workflow.yml
 .github/workflows/site.yml
 .github/workflows/status-report.yml
-.github/workflows/twitter-list.yml
 newshomepages/__init__.py
 newshomepages/accessibility.py
 newshomepages/altair_theme.py
 newshomepages/analyze.py
 newshomepages/archive.py
 newshomepages/batch.py
 newshomepages/discorder.py
```

### Comparing `newshomepages-0.0.8/newshomepages.egg-info/entry_points.txt` & `newshomepages-0.0.9/newshomepages.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.8/setup.py` & `newshomepages-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     If that issue is resolved, this method can be removed.
     """
     return ""
 
 
 setup(
     name="newshomepages",
-    description="A template for open-source Python software repositories",
+    description="An open-source archive that gathers, saves, shares and analyzes news homepages",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Ben Welsh",
     author_email="b@palewi.re",
     url="https://homepages.news",
     license="GPLv3",
     packages=find_packages(include=["newshomepages"]),
@@ -112,15 +112,17 @@
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Topic :: System :: Archiving",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: News/Diary",
     ],
     setup_requires=["setuptools_scm"],
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     project_urls={
         "Maintainer": "https://palewi.re/who-is-ben-welsh/",
         "Source": "https://github.com/palewire/news-homepages",
         "Tracker": "https://github.com/palewire/news-homepages/issues",
```

