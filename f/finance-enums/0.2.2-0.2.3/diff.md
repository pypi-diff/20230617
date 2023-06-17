# Comparing `tmp/finance_enums-0.2.2.tar.gz` & `tmp/finance_enums-0.2.3.tar.gz`

## Comparing `finance_enums-0.2.2.tar` & `finance_enums-0.2.3.tar`

### file list

```diff
@@ -1,326 +1,329 @@
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 finance_enums-0.2.2/local_dependencies/finance_enums/Cargo.toml
--rw-r--r--   0     1001      123     1587 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/Makefile
--rw-r--r--   0     1001      123        1 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/common/mod.rs
--rw-r--r--   0     1001      123   157760 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/country/iso3166.rs
--rw-r--r--   0     1001      123       34 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/country/mod.rs
--rw-r--r--   0     1001      123    11111 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/currency/iso4217.rs
--rw-r--r--   0     1001      123       33 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/currency/mod.rs
--rw-r--r--   0     1001      123     3782 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/exchange/iso10383.rs
--rw-r--r--   0     1001      123       87 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/exchange/mod.rs
--rw-r--r--   0     1001      123       44 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/instrument/iso10962.rs
--rw-r--r--   0     1001      123      470 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/instrument/mod.rs
--rw-r--r--   0     1001      123      351 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/lib.rs
--rw-r--r--   0     1001      123    22788 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry.rs
--rw-r--r--   0     1001      123    10841 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry_group.rs
--rw-r--r--   0     1001      123      314 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/mod.rs
--rw-r--r--   0     1001      123     5186 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/sector.rs
--rw-r--r--   0     1001      123    24096 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/subindustry.rs
--rw-r--r--   0     1001      123      252 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/bond.rs
--rw-r--r--   0     1001      123     1287 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/commodity.rs
--rw-r--r--   0     1001      123        1 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/currency.rs
--rw-r--r--   0     1001      123      319 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/equity.rs
--rw-r--r--   0     1001      123      662 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/fund.rs
--rw-r--r--   0     1001      123      441 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/future.rs
--rw-r--r--   0     1001      123      290 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/mod.rs
--rw-r--r--   0     1001      123      448 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/option.rs
--rw-r--r--   0     1001      123      362 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/security/security.rs
--rw-r--r--   0     1001      123      848 2023-06-15 20:52:19.000000 finance_enums-0.2.2/local_dependencies/finance_enums/src/trading/mod.rs
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 finance_enums-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123      414 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.bumpversion.cfg
--rw-r--r--   0     1001      123      147 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.gitattributes
--rw-r--r--   0     1001      123     3352 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123      834 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      595 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      206 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/dependabot.yml
--rw-r--r--   0     1001      123     1608 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/workflows/build.yml
--rw-r--r--   0     1001      123     4126 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0     1001      123     2284 2023-06-15 20:52:19.000000 finance_enums-0.2.2/.gitignore
--rw-r--r--   0     1001      123    11351 2023-06-15 20:52:19.000000 finance_enums-0.2.2/LICENSE
--rw-r--r--   0     1001      123     1990 2023-06-15 20:52:19.000000 finance_enums-0.2.2/Makefile
--rw-r--r--   0     1001      123     1246 2023-06-15 20:52:19.000000 finance_enums-0.2.2/README.md
--rw-r--r--   0     1001      123       52 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/__init__.py
--rw-r--r--   0     1001      123       52 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_all.py
--rw-r--r--   0     1001      123      195 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_country.py
--rw-r--r--   0     1001      123      429 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_currency.py
--rw-r--r--   0     1001      123      137 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_exchange.py
--rw-r--r--   0     1001      123        0 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_instrument.py
--rw-r--r--   0     1001      123      428 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_sector.py
--rw-r--r--   0     1001      123     1024 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_security.py
--rw-r--r--   0     1001      123      413 2023-06-15 20:52:19.000000 finance_enums-0.2.2/finance_enums/tests/test_trading.py
--rw-r--r--   0     1001      123      309 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AD.png
--rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AE.png
--rw-r--r--   0     1001      123      586 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AF.png
--rw-r--r--   0     1001      123      443 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AG.png
--rw-r--r--   0     1001      123      410 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AI.png
--rw-r--r--   0     1001      123      315 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AL.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AM.png
--rw-r--r--   0     1001      123      285 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AO.png
--rw-r--r--   0     1001      123      300 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AQ.png
--rw-r--r--   0     1001      123      150 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AR.png
--rw-r--r--   0     1001      123      469 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AS.png
--rw-r--r--   0     1001      123       93 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AT.png
--rw-r--r--   0     1001      123      405 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AU.png
--rw-r--r--   0     1001      123      176 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AW.png
--rw-r--r--   0     1001      123      155 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AX.png
--rw-r--r--   0     1001      123      165 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/AZ.png
--rw-r--r--   0     1001      123      321 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BA.png
--rw-r--r--   0     1001      123      235 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BB.png
--rw-r--r--   0     1001      123      246 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BD.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BE.png
--rw-r--r--   0     1001      123      173 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BF.png
--rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BG.png
--rw-r--r--   0     1001      123      189 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BH.png
--rw-r--r--   0     1001      123      394 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BI.png
--rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BJ.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BL.png
--rw-r--r--   0     1001      123      461 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BM.png
--rw-r--r--   0     1001      123      547 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BN.png
--rw-r--r--   0     1001      123      217 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BO.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BQ.png
--rw-r--r--   0     1001      123      438 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BR.png
--rw-r--r--   0     1001      123      181 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BS.png
--rw-r--r--   0     1001      123      570 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BT.png
--rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BV.png
--rw-r--r--   0     1001      123      111 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BW.png
--rw-r--r--   0     1001      123      206 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BY.png
--rw-r--r--   0     1001      123      378 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/BZ.png
--rw-r--r--   0     1001      123      259 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CA.png
--rw-r--r--   0     1001      123      365 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CC.png
--rw-r--r--   0     1001      123      350 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CD.png
--rw-r--r--   0     1001      123      246 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CF.png
--rw-r--r--   0     1001      123      330 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CG.png
--rw-r--r--   0     1001      123      113 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CH.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CI.png
--rw-r--r--   0     1001      123      487 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CK.png
--rw-r--r--   0     1001      123      186 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CL.png
--rw-r--r--   0     1001      123      158 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CM.png
--rw-r--r--   0     1001      123      214 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CN.png
--rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CO.png
--rw-r--r--   0     1001      123      123 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CR.png
--rw-r--r--   0     1001      123      240 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CU.png
--rw-r--r--   0     1001      123      267 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CV.png
--rw-r--r--   0     1001      123      189 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CW.png
--rw-r--r--   0     1001      123      508 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CX.png
--rw-r--r--   0     1001      123      318 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CY.png
--rw-r--r--   0     1001      123      273 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/CZ.png
--rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DE.png
--rw-r--r--   0     1001      123      358 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DJ.png
--rw-r--r--   0     1001      123      124 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DK.png
--rw-r--r--   0     1001      123      269 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DM.png
--rw-r--r--   0     1001      123      158 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DO.png
--rw-r--r--   0     1001      123      276 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/DZ.png
--rw-r--r--   0     1001      123      325 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EC.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EE.png
--rw-r--r--   0     1001      123      175 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EG.png
--rw-r--r--   0     1001      123      271 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/EH.png
--rw-r--r--   0     1001      123      465 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ER.png
--rw-r--r--   0     1001      123      273 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ES.png
--rw-r--r--   0     1001      123      324 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ET.png
--rw-r--r--   0     1001      123      130 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FI.png
--rw-r--r--   0     1001      123      456 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FJ.png
--rw-r--r--   0     1001      123      475 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FK.png
--rw-r--r--   0     1001      123      183 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FM.png
--rw-r--r--   0     1001      123      150 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FO.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/FR.png
--rw-r--r--   0     1001      123       98 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GA.png
--rw-r--r--   0     1001      123      490 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GB.png
--rw-r--r--   0     1001      123      417 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GD.png
--rw-r--r--   0     1001      123      155 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GE.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GF.png
--rw-r--r--   0     1001      123      184 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GG.png
--rw-r--r--   0     1001      123      180 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GH.png
--rw-r--r--   0     1001      123      288 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GI.png
--rw-r--r--   0     1001      123      302 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GL.png
--rw-r--r--   0     1001      123      110 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GM.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GN.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GP.png
--rw-r--r--   0     1001      123      305 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GQ.png
--rw-r--r--   0     1001      123      180 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GR.png
--rw-r--r--   0     1001      123      517 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GS.png
--rw-r--r--   0     1001      123      210 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GT.png
--rw-r--r--   0     1001      123      237 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GU.png
--rw-r--r--   0     1001      123      168 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GW.png
--rw-r--r--   0     1001      123      375 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/GY.png
--rw-r--r--   0     1001      123      321 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HK.png
--rw-r--r--   0     1001      123      405 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HM.png
--rw-r--r--   0     1001      123      137 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HN.png
--rw-r--r--   0     1001      123      262 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HR.png
--rw-r--r--   0     1001      123      171 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HT.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/HU.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ID.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IE.png
--rw-r--r--   0     1001      123      170 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IL.png
--rw-r--r--   0     1001      123      250 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IM.png
--rw-r--r--   0     1001      123      182 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IN.png
--rw-r--r--   0     1001      123      952 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IO.png
--rw-r--r--   0     1001      123      203 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IQ.png
--rw-r--r--   0     1001      123      356 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IR.png
--rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IS.png
--rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/IT.png
--rw-r--r--   0     1001      123      453 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JE.png
--rw-r--r--   0     1001      123      322 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JM.png
--rw-r--r--   0     1001      123      250 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JO.png
--rw-r--r--   0     1001      123      240 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/JP.png
--rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KE.png
--rw-r--r--   0     1001      123      327 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KG.png
--rw-r--r--   0     1001      123      271 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KH.png
--rw-r--r--   0     1001      123      604 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KI.png
--rw-r--r--   0     1001      123      413 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KM.png
--rw-r--r--   0     1001      123      618 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KN.png
--rw-r--r--   0     1001      123      233 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KP.png
--rw-r--r--   0     1001      123      447 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KR.png
--rw-r--r--   0     1001      123      195 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KW.png
--rw-r--r--   0     1001      123      456 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KY.png
--rw-r--r--   0     1001      123      331 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/KZ.png
--rw-r--r--   0     1001      123      173 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LA.png
--rw-r--r--   0     1001      123      308 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LB.png
--rw-r--r--   0     1001      123      261 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LC.png
--rw-r--r--   0     1001      123      199 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LI.png
--rw-r--r--   0     1001      123      492 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LK.png
--rw-r--r--   0     1001      123      205 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LR.png
--rw-r--r--   0     1001      123      209 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LS.png
--rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LT.png
--rw-r--r--   0     1001      123      116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LU.png
--rw-r--r--   0     1001      123      103 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LV.png
--rw-r--r--   0     1001      123      149 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/LY.png
--rw-r--r--   0     1001      123      190 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MA.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MC.png
--rw-r--r--   0     1001      123      249 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MD.png
--rw-r--r--   0     1001      123      335 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ME.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MF.png
--rw-r--r--   0     1001      123      122 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MG.png
--rw-r--r--   0     1001      123      520 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MH.png
--rw-r--r--   0     1001      123      418 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MK.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ML.png
--rw-r--r--   0     1001      123      280 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MM.png
--rw-r--r--   0     1001      123      243 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MN.png
--rw-r--r--   0     1001      123      311 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MO.png
--rw-r--r--   0     1001      123      450 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MP.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MQ.png
--rw-r--r--   0     1001      123      266 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MR.png
--rw-r--r--   0     1001      123      454 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MS.png
--rw-r--r--   0     1001      123      174 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MT.png
--rw-r--r--   0     1001      123      132 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MU.png
--rw-r--r--   0     1001      123      187 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MV.png
--rw-r--r--   0     1001      123      231 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MW.png
--rw-r--r--   0     1001      123      247 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MX.png
--rw-r--r--   0     1001      123      304 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MY.png
--rw-r--r--   0     1001      123      395 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/MZ.png
--rw-r--r--   0     1001      123      602 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NA.png
--rw-r--r--   0     1001      123      393 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NC.png
--rw-r--r--   0     1001      123      152 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NE.png
--rw-r--r--   0     1001      123      284 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NF.png
--rw-r--r--   0     1001      123       96 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NG.png
--rw-r--r--   0     1001      123      193 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NI.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NL.png
--rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NO.png
--rw-r--r--   0     1001      123      646 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NP.png
--rw-r--r--   0     1001      123      151 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NR.png
--rw-r--r--   0     1001      123      336 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NU.png
--rw-r--r--   0     1001      123      376 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/NZ.png
--rw-r--r--   0     1001      123      179 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/OM.png
--rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PA.png
--rw-r--r--   0     1001      123       96 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PE.png
--rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PF.png
--rw-r--r--   0     1001      123      377 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PG.png
--rw-r--r--   0     1001      123      319 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PH.png
--rw-r--r--   0     1001      123      295 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PK.png
--rw-r--r--   0     1001      123       92 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PL.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PM.png
--rw-r--r--   0     1001      123      556 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PN.png
--rw-r--r--   0     1001      123      296 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PR.png
--rw-r--r--   0     1001      123      293 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PS.png
--rw-r--r--   0     1001      123      354 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PT.png
--rw-r--r--   0     1001      123      239 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PW.png
--rw-r--r--   0     1001      123      190 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/PY.png
--rw-r--r--   0     1001      123      104 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/QA.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RE.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RO.png
--rw-r--r--   0     1001      123      398 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RS.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RU.png
--rw-r--r--   0     1001      123      212 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/RW.png
--rw-r--r--   0     1001      123      334 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SA.png
--rw-r--r--   0     1001      123      477 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SB.png
--rw-r--r--   0     1001      123      517 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SC.png
--rw-r--r--   0     1001      123      222 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SD.png
--rw-r--r--   0     1001      123      130 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SE.png
--rw-r--r--   0     1001      123      249 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SG.png
--rw-r--r--   0     1001      123      490 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SH.png
--rw-r--r--   0     1001      123      173 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SI.png
--rw-r--r--   0     1001      123      153 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SJ.png
--rw-r--r--   0     1001      123      326 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SK.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SL.png
--rw-r--r--   0     1001      123      362 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SM.png
--rw-r--r--   0     1001      123      158 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SN.png
--rw-r--r--   0     1001      123      198 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SO.png
--rw-r--r--   0     1001      123      215 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SR.png
--rw-r--r--   0     1001      123      264 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SS.png
--rw-r--r--   0     1001      123      254 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ST.png
--rw-r--r--   0     1001      123      195 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SV.png
--rw-r--r--   0     1001      123      419 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SX.png
--rw-r--r--   0     1001      123      182 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SY.png
--rw-r--r--   0     1001      123      436 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/SZ.png
--rw-r--r--   0     1001      123      414 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TC.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TD.png
--rw-r--r--   0     1001      123      328 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TF.png
--rw-r--r--   0     1001      123      248 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TG.png
--rw-r--r--   0     1001      123      114 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TH.png
--rw-r--r--   0     1001      123      196 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TJ.png
--rw-r--r--   0     1001      123      384 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TK.png
--rw-r--r--   0     1001      123      280 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TL.png
--rw-r--r--   0     1001      123      486 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TM.png
--rw-r--r--   0     1001      123      285 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TN.png
--rw-r--r--   0     1001      123      142 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TO.png
--rw-r--r--   0     1001      123      263 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TR.png
--rw-r--r--   0     1001      123      466 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TT.png
--rw-r--r--   0     1001      123      482 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TV.png
--rw-r--r--   0     1001      123      235 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TW.png
--rw-r--r--   0     1001      123      511 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/TZ.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UA.png
--rw-r--r--   0     1001      123      231 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UG.png
--rw-r--r--   0     1001      123      333 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UM.png
--rw-r--r--   0     1001      123      333 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/US.png
--rw-r--r--   0     1001      123      294 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UY.png
--rw-r--r--   0     1001      123      213 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/UZ.png
--rw-r--r--   0     1001      123      282 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VA.png
--rw-r--r--   0     1001      123      239 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VC.png
--rw-r--r--   0     1001      123      197 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VE.png
--rw-r--r--   0     1001      123      471 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VG.png
--rw-r--r--   0     1001      123      795 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VI.png
--rw-r--r--   0     1001      123      205 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VN.png
--rw-r--r--   0     1001      123      427 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/VU.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/WF.png
--rw-r--r--   0     1001      123      182 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/WS.png
--rw-r--r--   0     1001      123      100 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/YE.png
--rw-r--r--   0     1001      123      108 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/YT.png
--rw-r--r--   0     1001      123      406 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ZA.png
--rw-r--r--   0     1001      123      225 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ZM.png
--rw-r--r--   0     1001      123      295 2023-06-15 20:52:19.000000 finance_enums-0.2.2/flags/ZW.png
--rw-r--r--   0     1001      123    79321 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/GICS Map 2023.xlsx
--rw-r--r--   0     1001      123   509696 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/ISO10383_MIC.csv
--rw-r--r--   0     1001      123      402 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/flags_to_strings.py
--rw-r--r--   0     1001      123   149847 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/iso10383_generated.rs
--rw-r--r--   0     1001      123     4968 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/process_mics.py
--rw-r--r--   0     1001      123      577 2023-06-15 20:52:19.000000 finance_enums-0.2.2/helpers/scrape_flags.py
--rw-r--r--   0     1001      123     1526 2023-06-15 20:52:19.000000 finance_enums-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123    52004 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/country/mod.rs
--rw-r--r--   0     1001      123    23116 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/currency/mod.rs
--rw-r--r--   0     1001      123     4020 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/exchange/mod.rs
--rw-r--r--   0     1001      123        0 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/instrument/mod.rs
--rw-r--r--   0     1001      123     1302 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123    12919 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/industry.rs
--rw-r--r--   0     1001      123     6439 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/industry_group.rs
--rw-r--r--   0     1001      123      190 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/mod.rs
--rw-r--r--   0     1001      123     3215 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/sector.rs
--rw-r--r--   0     1001      123    27863 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/sector/subindustry.rs
--rw-r--r--   0     1001      123     2013 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/bond.rs
--rw-r--r--   0     1001      123     2113 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/commodity.rs
--rw-r--r--   0     1001      123        0 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/currency.rs
--rw-r--r--   0     1001      123     2392 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/equity.rs
--rw-r--r--   0     1001      123     5893 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/fund.rs
--rw-r--r--   0     1001      123      259 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/mod.rs
--rw-r--r--   0     1001      123     3948 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/option.rs
--rw-r--r--   0     1001      123     3290 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/security/security.rs
--rw-r--r--   0     1001      123     7342 2023-06-15 20:52:19.000000 finance_enums-0.2.2/src/trading/mod.rs
--rw-r--r--   0     1001      123    17385 2023-06-15 20:52:54.000000 finance_enums-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 finance_enums-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 finance_enums-0.2.3/local_dependencies/finance_enums/Cargo.toml
+-rw-r--r--   0     1001      123     1587 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/Makefile
+-rw-r--r--   0     1001      123        1 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/common/mod.rs
+-rw-r--r--   0     1001      123   158040 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/country/iso3166.rs
+-rw-r--r--   0     1001      123       34 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/country/mod.rs
+-rw-r--r--   0     1001      123    11111 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/currency/iso4217.rs
+-rw-r--r--   0     1001      123       33 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/currency/mod.rs
+-rw-r--r--   0     1001      123    27914 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/exchange/iso10383.rs
+-rw-r--r--   0     1001      123       87 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/exchange/mod.rs
+-rw-r--r--   0     1001      123       44 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/instrument/iso10962.rs
+-rw-r--r--   0     1001      123      470 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/instrument/mod.rs
+-rw-r--r--   0     1001      123      351 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/lib.rs
+-rw-r--r--   0     1001      123    22788 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/industry.rs
+-rw-r--r--   0     1001      123    10841 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/industry_group.rs
+-rw-r--r--   0     1001      123      314 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/mod.rs
+-rw-r--r--   0     1001      123     5186 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/sector.rs
+-rw-r--r--   0     1001      123    24096 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/subindustry.rs
+-rw-r--r--   0     1001      123      252 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/bond.rs
+-rw-r--r--   0     1001      123     1287 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/commodity.rs
+-rw-r--r--   0     1001      123        1 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/currency.rs
+-rw-r--r--   0     1001      123      319 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/equity.rs
+-rw-r--r--   0     1001      123      662 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/fund.rs
+-rw-r--r--   0     1001      123      441 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/future.rs
+-rw-r--r--   0     1001      123      290 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/mod.rs
+-rw-r--r--   0     1001      123      448 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/option.rs
+-rw-r--r--   0     1001      123      362 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/security.rs
+-rw-r--r--   0     1001      123     1071 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/trading/mod.rs
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 finance_enums-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123      414 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.bumpversion.cfg
+-rw-r--r--   0     1001      123      147 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.gitattributes
+-rw-r--r--   0     1001      123     3352 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123      834 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      595 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      206 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1608 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0     1001      123     4126 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123     2284 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.gitignore
+-rw-r--r--   0     1001      123    11351 2023-06-17 01:04:48.000000 finance_enums-0.2.3/LICENSE
+-rw-r--r--   0     1001      123     1990 2023-06-17 01:04:48.000000 finance_enums-0.2.3/Makefile
+-rw-r--r--   0     1001      123     1246 2023-06-17 01:04:48.000000 finance_enums-0.2.3/README.md
+-rw-r--r--   0     1001      123       52 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/__init__.py
+-rw-r--r--   0     1001      123       52 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_all.py
+-rw-r--r--   0     1001      123      195 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_country.py
+-rw-r--r--   0     1001      123      429 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_currency.py
+-rw-r--r--   0     1001      123      137 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_exchange.py
+-rw-r--r--   0     1001      123        0 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_instrument.py
+-rw-r--r--   0     1001      123      428 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_sector.py
+-rw-r--r--   0     1001      123     1024 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_security.py
+-rw-r--r--   0     1001      123      513 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_trading.py
+-rw-r--r--   0     1001      123      309 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AD.png
+-rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AE.png
+-rw-r--r--   0     1001      123      586 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AF.png
+-rw-r--r--   0     1001      123      443 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AG.png
+-rw-r--r--   0     1001      123      410 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AI.png
+-rw-r--r--   0     1001      123      315 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AL.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AM.png
+-rw-r--r--   0     1001      123      285 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AO.png
+-rw-r--r--   0     1001      123      300 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AQ.png
+-rw-r--r--   0     1001      123      150 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AR.png
+-rw-r--r--   0     1001      123      469 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AS.png
+-rw-r--r--   0     1001      123       93 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AT.png
+-rw-r--r--   0     1001      123      405 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AU.png
+-rw-r--r--   0     1001      123      176 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AW.png
+-rw-r--r--   0     1001      123      155 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AX.png
+-rw-r--r--   0     1001      123      165 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AZ.png
+-rw-r--r--   0     1001      123      321 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BA.png
+-rw-r--r--   0     1001      123      235 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BB.png
+-rw-r--r--   0     1001      123      246 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BD.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BE.png
+-rw-r--r--   0     1001      123      173 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BF.png
+-rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BG.png
+-rw-r--r--   0     1001      123      189 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BH.png
+-rw-r--r--   0     1001      123      394 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BI.png
+-rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BJ.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BL.png
+-rw-r--r--   0     1001      123      461 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BM.png
+-rw-r--r--   0     1001      123      547 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BN.png
+-rw-r--r--   0     1001      123      217 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BO.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BQ.png
+-rw-r--r--   0     1001      123      438 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BR.png
+-rw-r--r--   0     1001      123      181 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BS.png
+-rw-r--r--   0     1001      123      570 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BT.png
+-rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BV.png
+-rw-r--r--   0     1001      123      111 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BW.png
+-rw-r--r--   0     1001      123      206 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BY.png
+-rw-r--r--   0     1001      123      378 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BZ.png
+-rw-r--r--   0     1001      123      259 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CA.png
+-rw-r--r--   0     1001      123      365 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CC.png
+-rw-r--r--   0     1001      123      350 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CD.png
+-rw-r--r--   0     1001      123      246 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CF.png
+-rw-r--r--   0     1001      123      330 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CG.png
+-rw-r--r--   0     1001      123      113 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CH.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CI.png
+-rw-r--r--   0     1001      123      487 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CK.png
+-rw-r--r--   0     1001      123      186 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CL.png
+-rw-r--r--   0     1001      123      158 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CM.png
+-rw-r--r--   0     1001      123      214 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CN.png
+-rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CO.png
+-rw-r--r--   0     1001      123      123 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CR.png
+-rw-r--r--   0     1001      123      240 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CU.png
+-rw-r--r--   0     1001      123      267 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CV.png
+-rw-r--r--   0     1001      123      189 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CW.png
+-rw-r--r--   0     1001      123      508 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CX.png
+-rw-r--r--   0     1001      123      318 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CY.png
+-rw-r--r--   0     1001      123      273 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CZ.png
+-rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DE.png
+-rw-r--r--   0     1001      123      358 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DJ.png
+-rw-r--r--   0     1001      123      124 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DK.png
+-rw-r--r--   0     1001      123      269 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DM.png
+-rw-r--r--   0     1001      123      158 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DO.png
+-rw-r--r--   0     1001      123      276 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DZ.png
+-rw-r--r--   0     1001      123      325 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EC.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EE.png
+-rw-r--r--   0     1001      123      175 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EG.png
+-rw-r--r--   0     1001      123      271 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EH.png
+-rw-r--r--   0     1001      123      465 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ER.png
+-rw-r--r--   0     1001      123      273 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ES.png
+-rw-r--r--   0     1001      123      324 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ET.png
+-rw-r--r--   0     1001      123      130 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FI.png
+-rw-r--r--   0     1001      123      456 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FJ.png
+-rw-r--r--   0     1001      123      475 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FK.png
+-rw-r--r--   0     1001      123      183 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FM.png
+-rw-r--r--   0     1001      123      150 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FO.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FR.png
+-rw-r--r--   0     1001      123       98 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GA.png
+-rw-r--r--   0     1001      123      490 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GB.png
+-rw-r--r--   0     1001      123      417 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GD.png
+-rw-r--r--   0     1001      123      155 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GE.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GF.png
+-rw-r--r--   0     1001      123      184 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GG.png
+-rw-r--r--   0     1001      123      180 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GH.png
+-rw-r--r--   0     1001      123      288 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GI.png
+-rw-r--r--   0     1001      123      302 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GL.png
+-rw-r--r--   0     1001      123      110 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GM.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GN.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GP.png
+-rw-r--r--   0     1001      123      305 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GQ.png
+-rw-r--r--   0     1001      123      180 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GR.png
+-rw-r--r--   0     1001      123      517 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GS.png
+-rw-r--r--   0     1001      123      210 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GT.png
+-rw-r--r--   0     1001      123      237 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GU.png
+-rw-r--r--   0     1001      123      168 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GW.png
+-rw-r--r--   0     1001      123      375 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GY.png
+-rw-r--r--   0     1001      123      321 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HK.png
+-rw-r--r--   0     1001      123      405 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HM.png
+-rw-r--r--   0     1001      123      137 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HN.png
+-rw-r--r--   0     1001      123      262 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HR.png
+-rw-r--r--   0     1001      123      171 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HT.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HU.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ID.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IE.png
+-rw-r--r--   0     1001      123      170 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IL.png
+-rw-r--r--   0     1001      123      250 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IM.png
+-rw-r--r--   0     1001      123      182 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IN.png
+-rw-r--r--   0     1001      123      952 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IO.png
+-rw-r--r--   0     1001      123      203 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IQ.png
+-rw-r--r--   0     1001      123      356 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IR.png
+-rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IS.png
+-rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IT.png
+-rw-r--r--   0     1001      123      453 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JE.png
+-rw-r--r--   0     1001      123      322 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JM.png
+-rw-r--r--   0     1001      123      250 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JO.png
+-rw-r--r--   0     1001      123      240 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JP.png
+-rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KE.png
+-rw-r--r--   0     1001      123      327 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KG.png
+-rw-r--r--   0     1001      123      271 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KH.png
+-rw-r--r--   0     1001      123      604 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KI.png
+-rw-r--r--   0     1001      123      413 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KM.png
+-rw-r--r--   0     1001      123      618 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KN.png
+-rw-r--r--   0     1001      123      233 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KP.png
+-rw-r--r--   0     1001      123      447 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KR.png
+-rw-r--r--   0     1001      123      195 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KW.png
+-rw-r--r--   0     1001      123      456 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KY.png
+-rw-r--r--   0     1001      123      331 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KZ.png
+-rw-r--r--   0     1001      123      173 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LA.png
+-rw-r--r--   0     1001      123      308 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LB.png
+-rw-r--r--   0     1001      123      261 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LC.png
+-rw-r--r--   0     1001      123      199 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LI.png
+-rw-r--r--   0     1001      123      492 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LK.png
+-rw-r--r--   0     1001      123      205 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LR.png
+-rw-r--r--   0     1001      123      209 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LS.png
+-rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LT.png
+-rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LU.png
+-rw-r--r--   0     1001      123      103 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LV.png
+-rw-r--r--   0     1001      123      149 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LY.png
+-rw-r--r--   0     1001      123      190 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MA.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MC.png
+-rw-r--r--   0     1001      123      249 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MD.png
+-rw-r--r--   0     1001      123      335 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ME.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MF.png
+-rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MG.png
+-rw-r--r--   0     1001      123      520 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MH.png
+-rw-r--r--   0     1001      123      418 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MK.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ML.png
+-rw-r--r--   0     1001      123      280 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MM.png
+-rw-r--r--   0     1001      123      243 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MN.png
+-rw-r--r--   0     1001      123      311 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MO.png
+-rw-r--r--   0     1001      123      450 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MP.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MQ.png
+-rw-r--r--   0     1001      123      266 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MR.png
+-rw-r--r--   0     1001      123      454 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MS.png
+-rw-r--r--   0     1001      123      174 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MT.png
+-rw-r--r--   0     1001      123      132 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MU.png
+-rw-r--r--   0     1001      123      187 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MV.png
+-rw-r--r--   0     1001      123      231 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MW.png
+-rw-r--r--   0     1001      123      247 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MX.png
+-rw-r--r--   0     1001      123      304 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MY.png
+-rw-r--r--   0     1001      123      395 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MZ.png
+-rw-r--r--   0     1001      123      602 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NA.png
+-rw-r--r--   0     1001      123      393 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NC.png
+-rw-r--r--   0     1001      123      152 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NE.png
+-rw-r--r--   0     1001      123      284 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NF.png
+-rw-r--r--   0     1001      123       96 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NG.png
+-rw-r--r--   0     1001      123      193 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NI.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NL.png
+-rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NO.png
+-rw-r--r--   0     1001      123      646 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NP.png
+-rw-r--r--   0     1001      123      151 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NR.png
+-rw-r--r--   0     1001      123      336 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NU.png
+-rw-r--r--   0     1001      123      376 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NZ.png
+-rw-r--r--   0     1001      123      179 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/OM.png
+-rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PA.png
+-rw-r--r--   0     1001      123       96 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PE.png
+-rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PF.png
+-rw-r--r--   0     1001      123      377 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PG.png
+-rw-r--r--   0     1001      123      319 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PH.png
+-rw-r--r--   0     1001      123      295 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PK.png
+-rw-r--r--   0     1001      123       92 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PL.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PM.png
+-rw-r--r--   0     1001      123      556 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PN.png
+-rw-r--r--   0     1001      123      296 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PR.png
+-rw-r--r--   0     1001      123      293 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PS.png
+-rw-r--r--   0     1001      123      354 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PT.png
+-rw-r--r--   0     1001      123      239 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PW.png
+-rw-r--r--   0     1001      123      190 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PY.png
+-rw-r--r--   0     1001      123      104 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/QA.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RE.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RO.png
+-rw-r--r--   0     1001      123      398 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RS.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RU.png
+-rw-r--r--   0     1001      123      212 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RW.png
+-rw-r--r--   0     1001      123      334 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SA.png
+-rw-r--r--   0     1001      123      477 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SB.png
+-rw-r--r--   0     1001      123      517 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SC.png
+-rw-r--r--   0     1001      123      222 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SD.png
+-rw-r--r--   0     1001      123      130 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SE.png
+-rw-r--r--   0     1001      123      249 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SG.png
+-rw-r--r--   0     1001      123      490 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SH.png
+-rw-r--r--   0     1001      123      173 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SI.png
+-rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SJ.png
+-rw-r--r--   0     1001      123      326 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SK.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SL.png
+-rw-r--r--   0     1001      123      362 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SM.png
+-rw-r--r--   0     1001      123      158 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SN.png
+-rw-r--r--   0     1001      123      198 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SO.png
+-rw-r--r--   0     1001      123      215 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SR.png
+-rw-r--r--   0     1001      123      264 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SS.png
+-rw-r--r--   0     1001      123      254 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ST.png
+-rw-r--r--   0     1001      123      195 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SV.png
+-rw-r--r--   0     1001      123      419 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SX.png
+-rw-r--r--   0     1001      123      182 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SY.png
+-rw-r--r--   0     1001      123      436 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SZ.png
+-rw-r--r--   0     1001      123      414 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TC.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TD.png
+-rw-r--r--   0     1001      123      328 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TF.png
+-rw-r--r--   0     1001      123      248 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TG.png
+-rw-r--r--   0     1001      123      114 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TH.png
+-rw-r--r--   0     1001      123      196 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TJ.png
+-rw-r--r--   0     1001      123      384 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TK.png
+-rw-r--r--   0     1001      123      280 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TL.png
+-rw-r--r--   0     1001      123      486 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TM.png
+-rw-r--r--   0     1001      123      285 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TN.png
+-rw-r--r--   0     1001      123      142 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TO.png
+-rw-r--r--   0     1001      123      263 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TR.png
+-rw-r--r--   0     1001      123      466 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TT.png
+-rw-r--r--   0     1001      123      482 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TV.png
+-rw-r--r--   0     1001      123      235 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TW.png
+-rw-r--r--   0     1001      123      511 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TZ.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UA.png
+-rw-r--r--   0     1001      123      231 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UG.png
+-rw-r--r--   0     1001      123      333 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UM.png
+-rw-r--r--   0     1001      123      333 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/US.png
+-rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UY.png
+-rw-r--r--   0     1001      123      213 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UZ.png
+-rw-r--r--   0     1001      123      282 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VA.png
+-rw-r--r--   0     1001      123      239 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VC.png
+-rw-r--r--   0     1001      123      197 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VE.png
+-rw-r--r--   0     1001      123      471 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VG.png
+-rw-r--r--   0     1001      123      795 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VI.png
+-rw-r--r--   0     1001      123      205 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VN.png
+-rw-r--r--   0     1001      123      427 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VU.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/WF.png
+-rw-r--r--   0     1001      123      182 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/WS.png
+-rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/YE.png
+-rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/YT.png
+-rw-r--r--   0     1001      123      406 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ZA.png
+-rw-r--r--   0     1001      123      225 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ZM.png
+-rw-r--r--   0     1001      123      295 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ZW.png
+-rw-r--r--   0     1001      123     2658 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/CA_MIC.csv
+-rw-r--r--   0     1001      123    79321 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/GICS Map 2023.xlsx
+-rw-r--r--   0     1001      123   509696 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/ISO10383_MIC.csv
+-rw-r--r--   0     1001      123    11357 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/US_MIC.csv
+-rw-r--r--   0     1001      123    67904 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/atslist053123.pdf
+-rw-r--r--   0     1001      123      402 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/flags_to_strings.py
+-rw-r--r--   0     1001      123   149847 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/iso10383_generated.rs
+-rw-r--r--   0     1001      123     4968 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/process_mics.py
+-rw-r--r--   0     1001      123      577 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/scrape_flags.py
+-rw-r--r--   0     1001      123     1526 2023-06-17 01:04:48.000000 finance_enums-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123    52004 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/country/mod.rs
+-rw-r--r--   0     1001      123    23116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/currency/mod.rs
+-rw-r--r--   0     1001      123    12045 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/exchange/mod.rs
+-rw-r--r--   0     1001      123        0 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/instrument/mod.rs
+-rw-r--r--   0     1001      123     1350 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123    12919 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/industry.rs
+-rw-r--r--   0     1001      123     6439 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/industry_group.rs
+-rw-r--r--   0     1001      123      190 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/mod.rs
+-rw-r--r--   0     1001      123     3215 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/sector.rs
+-rw-r--r--   0     1001      123    27863 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/subindustry.rs
+-rw-r--r--   0     1001      123     2013 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/bond.rs
+-rw-r--r--   0     1001      123     2113 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/commodity.rs
+-rw-r--r--   0     1001      123        0 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/currency.rs
+-rw-r--r--   0     1001      123     2392 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/equity.rs
+-rw-r--r--   0     1001      123     5893 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/fund.rs
+-rw-r--r--   0     1001      123      259 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/mod.rs
+-rw-r--r--   0     1001      123     3948 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/option.rs
+-rw-r--r--   0     1001      123     3290 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/security.rs
+-rw-r--r--   0     1001      123     9354 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/trading/mod.rs
+-rw-r--r--   0     1001      123    17385 2023-06-17 01:05:20.000000 finance_enums-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 finance_enums-0.2.3/PKG-INFO
```

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/Cargo.toml` & `finance_enums-0.2.3/local_dependencies/finance_enums/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "finance_enums"
-version = "0.2.2"
+version = "0.2.3"
 authors = ["timkpaine <t.paine154@gmail.com>"]
 edition = "2021"
 license = "Apache-2.0"
 readme = "../README.md"
 repository = "https://github.com/timkpaine/finance-enums"
 description = "Standard Financial Enumerations"
```

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/Makefile` & `finance_enums-0.2.3/local_dependencies/finance_enums/Makefile`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/country/iso3166.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/country/iso3166.rs`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     VG,
     VI,
     WF,
     EH,
     YE,
     ZM,
     ZW,
+    XX, // INVALID
 }
 
 #[derive(
     Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
 )]
 #[strum(serialize_all = "UPPERCASE")]
 pub enum CountryCode3 {
@@ -507,14 +508,15 @@
     VGB,
     VIR,
     WLF,
     ESH,
     YEM,
     ZMB,
     ZWE,
+    XXX, // INVALID
 }
 
 impl CountryCode {
     pub fn str(&self) -> &'static str {
         match self {
             CountryCode::AF => "Afghanistan",
             CountryCode::AX => "Åland Islands",
@@ -761,14 +763,15 @@
             CountryCode::VG => "British Virgin Islands",
             CountryCode::VI => "U.S. Virgin Islands",
             CountryCode::WF => "Wallis and Futuna",
             CountryCode::EH => "Western Sahara",
             CountryCode::YE => "Yemen",
             CountryCode::ZM => "Zambia",
             CountryCode::ZW => "Zimbabwe",
+            CountryCode::XX => "Uncategorized",
         }
     }
 
     pub fn codethree(&self) -> CountryCode3 {
         match self {
             CountryCode::AF => CountryCode3::AFG,
             CountryCode::AX => CountryCode3::ALA,
@@ -1015,14 +1018,15 @@
             CountryCode::VG => CountryCode3::VGB,
             CountryCode::VI => CountryCode3::VIR,
             CountryCode::WF => CountryCode3::WLF,
             CountryCode::EH => CountryCode3::ESH,
             CountryCode::YE => CountryCode3::YEM,
             CountryCode::ZM => CountryCode3::ZMB,
             CountryCode::ZW => CountryCode3::ZWE,
+            CountryCode::XX => CountryCode3::XXX,
         }
     }
     pub fn flag(&self) -> &'static str {
         match self {
             CountryCode::TG => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAOCAMAAADzLXfBAAAAXVBMVEXSEDRvOkEAak7WKUrVIELxtsGHQzkzfj7UHD7vp7T54OX+/f30xM7hXnfnaRz/zgDVIUP++Pn////rl6fWJET42t/qjZ7vq7i3Viuaph/WJEXTEzbWJ0jtghXGkxomgcviAAAAVklEQVQY03XORw6AMAxE0SGU0EPvcP9jYqFsjCZv4cWXZRnwIqN8LeY9SWVkVgHyoqzqBq1TZLPrhxGkT/OyAtuuSD9OXPwf9uftPb87jgt2y8Fwof4CGe0LXp2aNUwAAAAASUVORK5CYII=",
             CountryCode::ME => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAMCAMAAAC+5dbKAAAAn1BMVEXppSbnfiHneiHjBhPiGBPeYRrkHhXiJRPjOhXjTRfldBnjUBfjNBbjLBTiXxflfhzjZhnjZBjkbxrkfBriZRfiZRrmnSG5dzCXfESrdTjmnyLiaxrhURbjkR2kgTyvgTe7hjHklBziOBThLRTiMRTZihyZiSfZjx3XThzaQhrjERPhcRfjUhnllh/jVRjbWx3fMhfjFBTjLRbieRriNBTDvIBbAAAAA3RSTlPp4eC7Kg8kAAAAXElEQVQY02NgYMQGGBiYmLEBJiRxFlY2LOLsHJxc3Dy8GOJ8/AKCQsIiGOKiYuISklLSGOIysnLyCopKGOLKKqpq6hqaGOJa2jq6evoGmO40NDI2wep+VH/hCAcAtckHktksxBYAAAAASUVORK5CYII=",
             CountryCode::LA => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAPBAMAAAD9gUllAAAAMFBMVEXOESaaFzYAKGgBKWlIZZNyiKwCKmmwvND///+vvNBWcZtVcJqEl7aDlrZxh6tHZJI1QmCYAAAAOElEQVQI12NgIA4IIoAAgxIQKLs6gygFMCe9ozMJzlnR0bEJzjnR0XEJuwyKHmW/zxDTUOwhDgAAdZIWfkb/TMAAAAAASUVORK5CYII=",
@@ -1268,14 +1272,15 @@
             CountryCode::CC => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAMCAMAAAC+5dbKAAAAq1BMVEUAgAAKhAAHggABgACStwD73gDGzAB5rQAZiQBaogBRngDn1wBKnAAtkQDKzAA2lAAeiwBgpACDsQDAyQB9rwBDkwCMtQBopwA5lQBxqgA3lQAPhQACgQD/4ADu2gDXqgD33QBbogDa0gAmjgAFgQA0lAA1lACaugA/lwCRtgDvzwDgugB4rQDNzQBhpAAUhwCfvAAEggAGggDMzQBOngDZ0gAojwAtkAA4lQCWLblvAAAAfUlEQVQY02NgYGBgZGLAAphZWNnYEVwOTiiDi5uHl48fLi4gCGUICYuIiokDGRKSUhARaRmwelk5eQWgekUlZRVVNZCIugbYfE0tbR0gravHwKBvYAhkqahA9DEagUhjoDgziGGC6i5OUzMjc2wOtpDkZ8AN4O5HA3D3YwcApG8HaL5sIQMAAAAASUVORK5CYII=",
             CountryCode::MH => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAMCAMAAAC+5dbKAAABGlBMVEUAOJMCOpQXPoN9WkABOZMaTJ4aP4LVcwXddQALQZg8Z6xmiL4rWqUFPJUcQIHWcwXddgHmmUI9aK3H0+f19/uyw94uXKYdQX+FXDvadALgghjttXf67Nv///8ZTJ5jhb3y9fni6PNQdrUVSJwmQnqRYDPbdAHddgLmmkT00ar+/Pr7/P0mVqOnutrf5vGWrdMXSp0oQ3iMXzbadQLggxr77d7u8viqvdtdgboRRZoEO5UoV6RIcLEqQ3eTYTHcdwT+/fvd5PGQqNBEbbASRpszRnGaYyzhhBz77+H8/f7M1+l/m8kqWaWbZTDoo1X22rv09fmodEPvv4jb29+Zr9RMc7MGPZY7SW60jGPFubN/msgzYKlyepNafLQNxpQRAAAAqUlEQVQY02NgAAJGBjTAxAwiWVhZUETZmNk5gBQnFzcPL0KUj5mfQ0AQqFpIWERUDCYqLiHJISUtI8vAIievIKuopAwWVVFVU9fQ1JKV1Qaq19HV0zcAiRoaGZtIm8rKmplbWAK5VtY2BlYMDLZ29hqaDrKOTs5wy1wYGFzd3KU9PL28fVBc5urr5x8gym2A6gvXwKDgkNAwNL+FR0RGRTNggJhYFwYsAABwIBQEctPXdgAAAABJRU5ErkJggg==",
             CountryCode::ZA => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAPCAMAAAA4caRkAAAAw1BMVEUAd0kEeUx3tp728/Hul5HgPjPgPDEHeUgpjWbF4Nb409DlW1HbryI/hz4BeEpmrZLy8u/ulpDgPzRNOAjkpBmZni4MekcgiGC62s7529nmYlkAAAAQDAKZbhHfsCFEiD1VpIbs8e7wn5nhQTZINAjhohmqoysSfEYYhFqt08T///8OCgKRaRDisSFNizt9Wg7/uBxZjTpFiT3o8PCBi8UGGowAFInLz+cuPp7q8fJ2gcAEGIvFyuQoOZzt8vR3gsACFooie8SHAAAAjklEQVQY03WQ1RLCUAxEF3d3AhR3aLHg8v9fRVoG2nunnMezmcwmAALBUDgS1UAMQDyRTOk+nZEgm8sXiqovlStVSWr1RlPx1Gp3DAnQ7fUHXk80HI0nEkxncxfb02K5WkODHExr4+P/zPvvlz5bp89uf+Afbv/jiT187z1frqz4z39ud1aB/c/H86VpfgM38h/ovgvjDAAAAABJRU5ErkJggg==",
             CountryCode::UY => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAPCAMAAAA4caRkAAAAhFBMVEX////9/Pvu48zj0a7t3sT+/v7X4PGqveLStX/Hn0S/kifRsmbr3cKEn9UAOKjr3sLIn0LFkw/YqhLBkB3dxY78+/rp2rzJoTzVpxHluBLAjxfIpVf17+fu4c3PrmKxgCPAkRzCljfq27f8+vf07eLdxJHZwIrgzKD17uOtv+NUesX7+fbjZKDmAAAAXUlEQVQY03XPRQ7AMBADQBdTZmbG//+vUm9RsnP2Wl6ApKiabsBkHMCwbMf14AccIIziJM1yIV+UVd20nVDfD+M0L6vQg20/zgv3w/lPXsnKRw6BHPktkyN7qDzhAyrrD7DyNXvrAAAAAElFTkSuQmCC",
             CountryCode::WF => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAPBAMAAAD9gUllAAAAD1BMVEUAJlRUbYz////eYG7OESZmtw3fAAAAGElEQVQI12NgYGBgVFJSUnZxcXFgGJIcANJDF8sUY7+rAAAAAElFTkSuQmCC",
             CountryCode::VU => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAOCAMAAADzLXfBAAAA3lBMVEUxBAyfDCfSEDS9mg4+MgQ4BA6qDSocFwKYfAu3lQ0zKANGBRG0DiwAAAAgGgKXewunhwwpHwRNBhO3Di0OCwEMCgErIwOmhwygggslGwNUBhW+Di9XRwavjgxJPAU3LAS2lA0eFANJBRKTCyWcDCeIbwoyKQQlHgKpiQw7MAS7mA6ykQ1nVAhdTAdcSwdeTAZgTwariwwvJgPNpw82LAQYFwQANBcAaC8AbzIHBgAGBQAhHgQAPBsAhz0AlUMmIgQANhgAgjoxKQQAMhYAfzk4LQQAKBIAeDYAJxIAdTUecIAlAAAAiElEQVQY023PRRbCQBBF0cIT4BPc3d1dCrf9b4jkMGhI9x2+QQmRw6lCLrfHq+o+TfcHgnIHQkY4Eo3JPZ5IptKZbM7W80ahiFJZq1RrdYHQaLbaADrdXn8gEIaj8UTVMZ3NrTmL5WotmH2zNffu9gf+9b3zeDrzP+uvy/XGdqTfH0+W0evNKh+yEyl2qr7/SAAAAABJRU5ErkJggg==",
             CountryCode::TJ => "iVBORw0KGgoAAAANSUhEUgAAABcAAAAMCAMAAAC+5dbKAAAAPFBMVEXMAADpkZHqkoz///////398sj+9tj+9NH855n//vz+9dP//fj87bf855v76aGSvpKVv4+qv3Cev4EAZgDBcqXWAAAAQ0lEQVQY02NgoBJgRAAmJDYDMwywsLKxssB5CHF2Zg4gxhDn5OLm4ebixFTPxsvHy4ZQzw8DAoJCggJwHoMwdkCqOAAUSggc7yfNgAAAAABJRU5ErkJggg==",
+            CountryCode::XX => "", // TODO
         }
     }
 }
 
 impl CountryCode3 {
     pub fn str(&self) -> &'static str {
         match self {
@@ -1524,14 +1529,15 @@
             CountryCode3::VGB => "British Virgin Islands",
             CountryCode3::VIR => "U.S. Virgin Islands",
             CountryCode3::WLF => "Wallis and Futuna",
             CountryCode3::ESH => "Western Sahara",
             CountryCode3::YEM => "Yemen",
             CountryCode3::ZMB => "Zambia",
             CountryCode3::ZWE => "Zimbabwe",
+            CountryCode3::XXX => "Uncategorized",
         }
     }
 
     pub fn twocode(&self) -> CountryCode {
         match self {
             CountryCode3::AFG => CountryCode::AF,
             CountryCode3::ALA => CountryCode::AX,
@@ -1778,14 +1784,15 @@
             CountryCode3::VGB => CountryCode::VG,
             CountryCode3::VIR => CountryCode::VI,
             CountryCode3::WLF => CountryCode::WF,
             CountryCode3::ESH => CountryCode::EH,
             CountryCode3::YEM => CountryCode::YE,
             CountryCode3::ZMB => CountryCode::ZM,
             CountryCode3::ZWE => CountryCode::ZW,
+            CountryCode3::XXX => CountryCode::XX,
         }
     }
 }
 
 // AF,AFG,Afghanistan,AF,AFG
 // AX,ALA,Åland Islands,AX,ALA
 // AL,ALB,Albania,AL,ALB
```

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/currency/iso4217.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/currency/iso4217.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/industry.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/industry_group.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/industry_group.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/sector.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/sector.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/sector/subindustry.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/subindustry.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/security/commodity.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/security/commodity.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/security/fund.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/security/fund.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/local_dependencies/finance_enums/src/trading/mod.rs` & `finance_enums-0.2.3/local_dependencies/finance_enums/src/trading/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -34,7 +34,18 @@
 #[strum(serialize_all = "PascalCase")]
 pub enum OrderFlag {
     None,
     FillOrKill,
     ImmediateOrCancel,
     AllOrNone,
 }
+
+#[derive(
+    Copy, Clone, Debug, Deserialize, Display, EnumIter, EnumString, Eq, PartialEq, Serialize,
+)]
+#[strum(serialize_all = "PascalCase")]
+pub enum TradingType {
+    Live,
+    Paper,
+    Simulation,
+    Backtest,
+}
```

### Comparing `finance_enums-0.2.2/Cargo.toml` & `finance_enums-0.2.3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/.github/CODE_OF_CONDUCT.md` & `finance_enums-0.2.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `finance_enums-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `finance_enums-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/.github/workflows/build.yml` & `finance_enums-0.2.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/.github/workflows/publish.yml` & `finance_enums-0.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/.gitignore` & `finance_enums-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/LICENSE` & `finance_enums-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/Makefile` & `finance_enums-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/README.md` & `finance_enums-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/finance_enums/tests/test_security.py` & `finance_enums-0.2.3/finance_enums/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/AF.png` & `finance_enums-0.2.3/flags/AF.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/BN.png` & `finance_enums-0.2.3/flags/BN.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/BT.png` & `finance_enums-0.2.3/flags/BT.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/GS.png` & `finance_enums-0.2.3/flags/GS.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/IO.png` & `finance_enums-0.2.3/flags/IO.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/KI.png` & `finance_enums-0.2.3/flags/KI.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/KN.png` & `finance_enums-0.2.3/flags/KN.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/MH.png` & `finance_enums-0.2.3/flags/MH.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/NA.png` & `finance_enums-0.2.3/flags/NA.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/NP.png` & `finance_enums-0.2.3/flags/NP.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/PN.png` & `finance_enums-0.2.3/flags/PN.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/SC.png` & `finance_enums-0.2.3/flags/SC.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/flags/VI.png` & `finance_enums-0.2.3/flags/VI.png`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/helpers/GICS Map 2023.xlsx` & `finance_enums-0.2.3/helpers/GICS Map 2023.xlsx`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/helpers/ISO10383_MIC.csv` & `finance_enums-0.2.3/helpers/ISO10383_MIC.csv`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/helpers/iso10383_generated.rs` & `finance_enums-0.2.3/helpers/iso10383_generated.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/helpers/process_mics.py` & `finance_enums-0.2.3/helpers/process_mics.py`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/helpers/scrape_flags.py` & `finance_enums-0.2.3/helpers/scrape_flags.py`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/pyproject.toml` & `finance_enums-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "finance-enums"
 authors = [{name = "Tim Paine", email = "t.paine154@gmail.com"}]
 description="Standard Financial Enumerations"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `finance_enums-0.2.2/src/country/mod.rs` & `finance_enums-0.2.3/src/country/mod.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/currency/mod.rs` & `finance_enums-0.2.3/src/currency/mod.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/lib.rs` & `finance_enums-0.2.3/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 mod trading;
 
 use country::Country;
 use currency::Currency;
 use exchange::Exchange;
 use sector::{Sector, IndustryGroup, Industry, SubIndustry};
 use security::{SecurityType, EquityType, OptionType, BondType, CommodityType, FundType, OptionExerciseType, FundSubType, MutualFundEndedness};
-use trading::{OrderType, Side, TimeInForce, OrderFlag};
+use trading::{OrderType, Side, TimeInForce, OrderFlag, TradingType};
 
 #[pymodule]
 fn finance_enums(_py: Python, m: &PyModule) -> PyResult<()> {
     // Country
     m.add_class::<Country>()?;
 
     // Currency
@@ -43,9 +43,10 @@
     m.add_class::<FundSubType>()?;
     m.add_class::<MutualFundEndedness>()?;
 
     m.add_class::<OrderType>()?;
     m.add_class::<Side>()?;
     m.add_class::<TimeInForce>()?;
     m.add_class::<OrderFlag>()?;
+    m.add_class::<TradingType>()?;
     Ok(())
 }
```

### Comparing `finance_enums-0.2.2/src/sector/industry.rs` & `finance_enums-0.2.3/src/sector/industry.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/sector/industry_group.rs` & `finance_enums-0.2.3/src/sector/industry_group.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/sector/sector.rs` & `finance_enums-0.2.3/src/sector/sector.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/sector/subindustry.rs` & `finance_enums-0.2.3/src/sector/subindustry.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/security/bond.rs` & `finance_enums-0.2.3/src/security/bond.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/security/commodity.rs` & `finance_enums-0.2.3/src/security/commodity.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/security/equity.rs` & `finance_enums-0.2.3/src/security/equity.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/security/fund.rs` & `finance_enums-0.2.3/src/security/fund.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/security/option.rs` & `finance_enums-0.2.3/src/security/option.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/security/security.rs` & `finance_enums-0.2.3/src/security/security.rs`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.2/src/trading/mod.rs` & `finance_enums-0.2.3/src/trading/mod.rs`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use pyo3::prelude::*;
 use pyo3::class::basic::CompareOp;
 use pyo3::types::PyType;
 use strum::IntoEnumIterator;
 use std::str::FromStr;
 
-use finance_enums::{OrderType as BaseOrderType, Side as BaseSide, TimeInForce as BaseTimeInForce, OrderFlag as BaseOrderFlag};
+use finance_enums::{OrderType as BaseOrderType, Side as BaseSide, TimeInForce as BaseTimeInForce, OrderFlag as BaseOrderFlag, TradingType as BaseTradingType};
 
 
 #[pyclass]
 pub struct OrderType {
     pub typ: BaseOrderType
 }
 
@@ -272,7 +272,82 @@
     #[classattr]
     fn AllOrNone() -> OrderFlag {
         OrderFlag {
             typ: BaseOrderFlag::AllOrNone
         }
     }
 }
+
+
+#[pyclass]
+pub struct TradingType {
+    pub typ: BaseTradingType
+}
+
+#[pymethods]
+impl TradingType {
+    #[new]
+    fn py_new(value: String) -> PyResult<Self> {
+        Ok(
+            TradingType {
+                typ: BaseTradingType::from_str(value.as_str()).unwrap()
+            }
+        )
+    }
+    
+    fn __str__(&self) -> PyResult<String>   {
+        Ok(format!("{}", self.typ.to_string()))
+    }
+    
+    fn __repr__(&self) -> PyResult<String>   {
+        Ok(format!("TradingType<{}>", self.typ.to_string()))
+    }
+    
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Lt => Ok(self.typ.to_string() < other.typ.to_string()),
+            CompareOp::Le => Ok(self.typ.to_string() <= other.typ.to_string()),
+            CompareOp::Eq => Ok(self.typ == other.typ),
+            CompareOp::Ne => Ok(self.typ != other.typ),
+            CompareOp::Gt => Ok(self.typ.to_string() > other.typ.to_string()),
+            CompareOp::Ge => Ok(self.typ.to_string() >= other.typ.to_string()),
+        }
+    }
+    
+    #[classmethod]
+    fn __len__(_cls: &PyType) -> PyResult<usize> {
+        Ok(BaseTradingType::iter().count())
+    }
+    
+    // TODO figure out how to make a class iterator,
+    // is way too complicated in pyo3 rn
+    #[staticmethod]
+    fn members() -> Vec<TradingType> {
+        BaseTradingType::iter().map(|item: BaseTradingType| TradingType{typ: item} ).collect()
+    }
+
+
+    #[classattr]
+    fn Live() -> TradingType {
+        TradingType {
+            typ: BaseTradingType::Live
+        }
+    }
+    #[classattr]
+    fn Paper() -> TradingType {
+        TradingType {
+            typ: BaseTradingType::Paper
+        }
+    }
+    #[classattr]
+    fn Backtest() -> TradingType {
+        TradingType {
+            typ: BaseTradingType::Backtest
+        }
+    }
+    #[classattr]
+    fn Simulation() -> TradingType {
+        TradingType {
+            typ: BaseTradingType::Simulation
+        }
+    }
+}
```

### Comparing `finance_enums-0.2.2/Cargo.lock` & `finance_enums-0.2.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 dependencies = [
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "finance_enums"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "casey",
  "chrono",
  "num",
  "serde",
  "serde_json",
  "strum",
@@ -431,17 +431,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `finance_enums-0.2.2/PKG-INFO` & `finance_enums-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance-enums
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

