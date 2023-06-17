# Comparing `tmp/naludaq-0.18.0.tar.gz` & `tmp/naludaq-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.18.0.tar", last modified: Thu Jun  1 23:50:03 2023, max compression
+gzip compressed data, was "naludaq-0.19.0.tar", last modified: Sat Jun 17 02:51:40 2023, max compression
```

## Comparing `naludaq-0.18.0.tar` & `naludaq-0.19.0.tar`

### file list

```diff
@@ -1,251 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-01 23:49:47.000000 naludaq-0.18.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-01 23:50:03.697728 naludaq-0.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-01 23:49:47.000000 naludaq-0.18.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 23:49:47.000000 naludaq-0.18.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:50:03.697728 naludaq-0.18.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-01 23:49:47.000000 naludaq-0.18.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.669728 naludaq-0.18.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.673728 naludaq-0.18.0/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.673728 naludaq-0.18.0/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.677728 naludaq-0.18.0/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/_fpga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/chip_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.681728 naludaq-0.18.0/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.685728 naludaq-0.18.0/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.689728 naludaq-0.18.0/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/ftdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.693728 naludaq-0.18.0/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/aav3.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/_new/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_acq.py
--rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/threshold_scan/threshold_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 23:49:47.000000 naludaq-0.18.0/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.673728 naludaq-0.18.0/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 23:50:03.000000 naludaq-0.18.0/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:50:03.697728 naludaq-0.18.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-01 23:49:47.000000 naludaq-0.18.0/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-17 02:51:24.000000 naludaq-0.19.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-06-17 02:51:40.535666 naludaq-0.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-06-17 02:51:24.000000 naludaq-0.19.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-17 02:51:24.000000 naludaq-0.19.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 02:51:40.535666 naludaq-0.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-17 02:51:24.000000 naludaq-0.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.499665 naludaq-0.19.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36060 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.507665 naludaq-0.19.0/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.507665 naludaq-0.19.0/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.511665 naludaq-0.19.0/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/asocv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.515665 naludaq-0.19.0/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.519665 naludaq-0.19.0/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.523666 naludaq-0.19.0/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.527665 naludaq-0.19.0/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/lookup_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/lookup_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/lookup_table/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/lookup_table/lookup_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.531665 naludaq-0.19.0/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/aav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/_new/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_acq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/threshold_scan/threshold_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-17 02:51:24.000000 naludaq-0.19.0/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.503665 naludaq-0.19.0/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 02:51:40.000000 naludaq-0.19.0/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:51:40.535666 naludaq-0.19.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 02:51:24.000000 naludaq-0.19.0/tests/test_naludaq.py
```

### Comparing `naludaq-0.18.0/LICENSE.txt` & `naludaq-0.19.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/PKG-INFO` & `naludaq-0.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.18.0
+Version: 0.19.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -82,15 +82,15 @@
 
 ```
 pip install -e .[dev]
 ```
 
 The package can now be imported in your project and edited in your favorite editor, [VS Code](https://code.visualstudio.com/)
 
-## Development wtih gigabit ethernet backend
+## Development with gigabit ethernet backend
 
 To use the gigabit ethernet backend you will need to install the `naludaq_rs` package.
 
 1. Clone the package from GitHub
 2. install the package as an editable package. See instructions in the `naludaq_rs` package.
 
 
@@ -104,14 +104,18 @@
 pre-commit install
 ```
 
 The hooks will run automatically when you commit changes to the repository.
 
 The code MUST run the pre-commit hooks before commiting. If the hooks fail, the commit will be rejected.
 
+# Examples
+
+See the [example repository](https://github.com/NaluScientific/naluexamples).
+
 # Development Use
 
 Once the package is installed it's now possible to start using the package.
 There is a boilerplate interface named `Naludaq` in `naludaq` it contains basic functionality.
 It's a good starting point to get the software started.
 If more advanced scripts are required please continue reading below.
 A datasheet for the board is also required to understand the registers and the commands.
```

### Comparing `naludaq-0.18.0/README.md` & `naludaq-0.19.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 ```
 pip install -e .[dev]
 ```
 
 The package can now be imported in your project and edited in your favorite editor, [VS Code](https://code.visualstudio.com/)
 
-## Development wtih gigabit ethernet backend
+## Development with gigabit ethernet backend
 
 To use the gigabit ethernet backend you will need to install the `naludaq_rs` package.
 
 1. Clone the package from GitHub
 2. install the package as an editable package. See instructions in the `naludaq_rs` package.
 
 
@@ -85,14 +85,18 @@
 pre-commit install
 ```
 
 The hooks will run automatically when you commit changes to the repository.
 
 The code MUST run the pre-commit hooks before commiting. If the hooks fail, the commit will be rejected.
 
+# Examples
+
+See the [example repository](https://github.com/NaluScientific/naluexamples).
+
 # Development Use
 
 Once the package is installed it's now possible to start using the package.
 There is a boilerplate interface named `Naludaq` in `naludaq` it contains basic functionality.
 It's a good starting point to get the software started.
 If more advanced scripts are required please continue reading below.
 A datasheet for the board is also required to understand the registers and the commands.
```

### Comparing `naludaq-0.18.0/pyproject.toml` & `naludaq-0.19.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 description = "Backend package for Nalu Scientific hardware"
 readme = "README.md"
 dynamic = ["version"]
 requires-python = ">=3.9"
 dependencies = [
   "naluconfigs>=11.0.0",
   "ftd3xx>=1.0",
-  "naludaq_rs>=0.1.5",
+  "naludaq_rs>=0.1.9",
   "deprecation",
   "ftd2xx>=1.1.2",
   "h5py",
   "numpy<1.24",
   "pyserial==3.4",
   "pyyaml>=5.1.1",
   "scikit-learn==1.1.3",
```

### Comparing `naludaq-0.18.0/setup.py` & `naludaq-0.19.0/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/client.py` & `naludaq-0.19.0/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/context.py` & `naludaq-0.19.0/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/exceptions.py` & `naludaq-0.19.0/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/managers/config.py` & `naludaq-0.19.0/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/managers/connection.py` & `naludaq-0.19.0/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/managers/io.py` & `naludaq-0.19.0/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/backend/models/acquisition.py` & `naludaq-0.19.0/src/naludaq/backend/models/acquisition.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,56 +100,55 @@
         return self.length
 
     def __getitem__(self, index: "int | slice") -> "bytes | list[bytes]":
         """Get events from the remote"""
         if isinstance(index, int):
             return self.raw_event(index)
         if isinstance(index, slice):
-            return [
-                self.raw_event(x) for x in range(index.start, index.stop, index.step)
-            ]
+            start, stop, step = index.indices(self.length)
+            return [self.raw_event(x) for x in range(start, stop, step)]
         raise TypeError("Index must be int or slice")
 
     def __iter__(self) -> Iterator[dict]:
         """Iterate over raw events"""
         return (self[i] for i in range(len(self)))
 
     @property
     def length(self) -> int:
         """Get the number of events in the acquisition"""
-        info = self._get_info_or_raise()
+        info = self._get_info_or_raise(len=True)
         return info["len"]
 
     @property
     def path(self) -> str:
         """Get the path to the acquisition on the remote"""
-        return self._get_info_or_raise()["path"]
+        return self._get_info_or_raise(path=True)["path"]
 
     @property
     def metadata(self) -> dict:
         """Get the acquisition metadata."""
         cache = RemoteAcquisition._METADATA_CACHE
         key = self._cache_key()
         metadata = cache.get(key, None)
         if metadata is None:
-            info = self._get_info_or_raise()
+            info = self._get_info_or_raise(metadata=True)
             metadata = yaml.safe_load(info["metadata"])
             cache[key] = metadata
         return metadata
 
     @property
     def params(self) -> dict:
         """Get params from the acq metadata"""
         return self.metadata["params"]
 
     @property
     def exists(self) -> bool:
         """Checks if this acquisition exists on the remote"""
         try:
-            _ = self._get_info_or_raise()
+            _ = self.length
         except BackendError:
             return False
         return True
 
     @property
     def readout_metadata(self) -> "dict | None":
         """Get/set the readout metadata for this acquisition"""
@@ -325,19 +324,33 @@
     def set_output(self):
         """Use this acquisition as the output for readouts"""
         self.context.client.put(
             "/acq/output",
             params={"name": self._name},
         )
 
-    def _get_info_or_raise(self) -> dict:
+    def _get_info_or_raise(
+        self,
+        len: bool = False,
+        path: bool = False,
+        metadata: bool = False,
+        chunk_count: bool = False,
+        total_size: bool = False,
+    ) -> dict:
         """Retrieve information about this acquisition"""
         return self.context.client.get_json(
             "acq/show",
-            params={"name": self._name},
+            params={
+                "name": self._name,
+                "len": int(len),
+                "path": int(path),
+                "metadata": int(metadata),
+                "chunk_count": int(chunk_count),
+                "total_size": int(total_size),
+            },
         )
 
     def invalidate_cache(self):
         """Invalidate the misc data cache for this acquisition."""
         cache = RemoteAcquisition._MISC_DATA_CACHE
         try:
             del cache[self._cache_key()]
```

### Comparing `naludaq-0.18.0/src/naludaq/backend/models/device.py` & `naludaq-0.19.0/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/__init__.py` & `naludaq-0.19.0/src/naludaq/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/board_inits.py` & `naludaq-0.19.0/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.19.0/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.19.0/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/_UART.py` & `naludaq-0.19.0/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/_USB.py` & `naludaq-0.19.0/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/base_connection.py` & `naludaq-0.19.0/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.19.0/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/tcp.py` & `naludaq-0.19.0/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/connections/udp.py` & `naludaq-0.19.0/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/__init__.py` & `naludaq-0.19.0/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.19.0/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.19.0/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.19.0/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.19.0/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.19.0/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.19.0/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.19.0/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/board/params.py` & `naludaq-0.19.0/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/__init__.py` & `naludaq-0.19.0/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/_chip.py` & `naludaq-0.19.0/src/naludaq/communication/_chip.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/_common.py` & `naludaq-0.19.0/src/naludaq/communication/_common.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/_fpga.py` & `naludaq-0.19.0/src/naludaq/communication/_fpga.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/analog_registers.py` & `naludaq-0.19.0/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/chip_selection.py` & `naludaq-0.19.0/src/naludaq/communication/chip_selection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/control_registers.py` & `naludaq-0.19.0/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/digital_registers.py` & `naludaq-0.19.0/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/i2c.py` & `naludaq-0.19.0/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/i2c_registers.py` & `naludaq-0.19.0/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/communication/registers.py` & `naludaq-0.19.0/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.19.0/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.19.0/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/board/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 All functions to communicate with the Nalu boards are
 collected here. The Facade naludaq is intended to simplify
 the interface for general use.
 """
 import logging
 
 from .aodsoc import BoardControllerAodsoc
+from .asocv3 import BoardControllerAsocv3
 from .default import BoardController
 from .hdsoc import HDSoCBoardController
 from .oleas import BoardControllerOleas
 from .trbhm import TrbhmBoardController
 from .udc import UDCBoardController
 from .upac import UpacBoardController
 from .upac96 import UPAC96BoardController
@@ -25,14 +26,15 @@
         board (Board): the board object.
 
     Returns:
         The appropriate BoardController for the given board.
     """
     return {
         # 'aodsoc_aods': BoardControllerAodsoc,
+        "asocv3": BoardControllerAsocv3,
         "aodsoc_aods": BoardControllerOleas,
         "aodsoc_asoc": BoardControllerAodsoc,
         "hdsocv1": HDSoCBoardController,
         "hdsocv1_evalr1": HDSoCBoardController,
         "hdsocv1_evalr2": HDSoCBoardController,
         "trbhm": TrbhmBoardController,
         "udc16": UDCBoardController,
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/board/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/default.py` & `naludaq-0.19.0/src/naludaq/controllers/board/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,17 @@
         - data_sel(1 downto 0) = acq type
 
         """
         readout_params = self._validate_readout_params(
             trig, lb, acq, dig_head, ped, readoutEn, singleEv
         )
         cmd = self._generate_start_readout_cmd(readout_params)
-        LOGGER.debug("Sending command: %s", cmd)
+        LOGGER.debug("READOUT command: %s", cmd)
 
-        if self.board.using_new_backend:
-            BoardIoManager(self.board).write(cmd)
-        else:
-            self.board.connection.send(cmd)
+        self._send_command(cmd)
 
     @staticmethod
     def _validate_readout_params(
         trig, lb, acq, dig_head, ped, readoutEn, singleEv
     ) -> dict:
         for name, in_val in {"trig": trig, "lb": lb, "acq": acq, "ped": ped}.items():
             if not isinstance(in_val, str):
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/oleas.py` & `naludaq-0.19.0/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.19.0/src/naludaq/controllers/board/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/udc.py` & `naludaq-0.19.0/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/upac.py` & `naludaq-0.19.0/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/board/upac96.py` & `naludaq-0.19.0/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.19.0/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/connection/upac.py` & `naludaq-0.19.0/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.19.0/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 thus they need to be intialized and operated differently.
 
 License: LGPL v3
 See LICENSE.txt
 """
 from naludaq.helpers.exceptions import InvalidBoardModelError
 
+from .aardvarcv3 import DacControllerAardvarcv3
 from .ad5671 import DACControllerAD5671
 from .ad5675 import DACControllerAD5675
 from .base import BaseDACController as _DACController
 from .dac7578 import DACControllerDAC7578
 from .hdsoc import DACControllerHDSoC
 from .trbhm import DACControllerTRBHM
 from .upac32 import DacControllerUpac32
@@ -40,16 +41,16 @@
         InvalidBoardModelError if the given board does not have
             a DAC controller
     """
     if not board.is_feature_enabled("ext_dac"):
         raise InvalidBoardModelError("The given board does not support DAC control")
 
     controller = {
-        "aardvarcv3": DACControllerDAC7578,
-        "aardvarcv4": DACControllerDAC7578,
+        "aardvarcv3": DacControllerAardvarcv3,
+        "aardvarcv4": DacControllerAardvarcv3,
         "aodsv1": DACControllerAD5671,
         "aodsv2_eval": DACControllerAD5671,
         "asocv3": DACControllerAD5671,
         "hdsocv1": DACControllerHDSoC,
         "hdsocv1_evalr1": DACControllerHDSoC,
         "hdsocv1_evalr2": DACControllerHDSoC,
         "trbhm": DACControllerTRBHM,
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,46 +58,48 @@
             self._broadcast_to_all_channels()
             return
 
         self._write_to_channels(channels)
 
     def _write_to_channels(self, channels: List[int]) -> None:
         """Writes the external dac values per channel in channels"""
-
-        rw = 0
         LOGGER.info(
             f"Setting channels {channels} to: {[self.board.dac_values[channel] for channel in channels]}"
         )
-
         for channel in channels:
             value = self.board.dac_values[channel]
             addr = self._address_mapping[channel]
             words = self._get_write_words(channel, value)
-
-            LOGGER.debug(
-                "Sent DAC Command - ADDR: %s, WORDS: %s", (addr << 1) | rw, words
-            )
-            if not sendI2cCommand(self.board, (addr << 1) | rw, words):
-                raise ConnectionError("Failed to write I2C DAC")
-            time.sleep(self._send_delay)
+            self._send_command(addr, words)
 
     def _broadcast_to_all_channels(self):
         """Broadcast  to every channel on EVERY ext. DAC chip."""
-        rw = 0
         unique_addrs = self._get_unique_addresses()
-
         for addr in unique_addrs:
             addr = int(addr)
             value = self.board.dac_values[0]
             words = self._get_broadcast_words(value)
             LOGGER.info("Broadcasting DAC value: %s to DAC %s", value, addr)
-            LOGGER.debug("Sent DAC Command: %s", words)
-            if not sendI2cCommand(self.board, (addr << 1) | rw, words):
-                raise ConnectionError("Failed to write I2C DAC")
-            time.sleep(self._send_delay)
+            self._send_command(addr, words)
+
+    def _send_command(self, addr: int, words: list[str], rw: int = 0) -> None:
+        """Send the given words to the DAC at the given address.
+
+        Args:
+            addr (int): the address of the DAC to send the words to.
+            words (List[str]): the words to send to the DAC.
+            rw (int): r/w bit (0 = write, 1 = read)
+
+        Raises:
+            ConnectionError if the I2C commands could not be sent
+        """
+        LOGGER.debug("Sent DAC Command - ADDR: %s, WORDS: %s", (addr << 1) | rw, words)
+        if not sendI2cCommand(self.board, (addr << 1) | rw, words):
+            raise ConnectionError("Failed to write I2C DAC")
+        time.sleep(self._send_delay)
 
     def _get_write_words(self, channel: int, value: int) -> List[str]:
         """Get words to write to set the DAC value for a channel.
 
         Args:
             channel (int): the channel to set the DAC value for.
             value (int): the DAC value.
@@ -108,15 +110,14 @@
         return [
             f"{self._write_cmd:04b}{self._channel_mapping[channel]:04b}",
             f"{(value >> 4 & 0xFF):08b}",
             f"{(value << 4 & 0xFF):08b}",
         ]
 
     def _get_broadcast_words(self, value: int) -> str:
-
         return [
             f"{self._write_cmd:04b}{0b1111:04b}",
             f"{(value >> 4 & 0xFF):08b}",
             f"{(value << 4 & 0xFF):08b}",
         ]
 
     def _get_unique_addresses(self):
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.19.0/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.19.0/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.19.0/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             params = self._board.params["peripherals"][name]
         except KeyError:
             raise NotImplementedError(
                 f"{name} readout functionality has not been implemented for {self.board.model}"
             )
         return params
 
-    def _read_MCP3426_ADC(self, chan, addr, bits=16, gain=1):
+    def _read_MCP3426_ADC(self, chan, addr, bits=16, gain=1, *args, **kwargs):
         """
         MCP3426/7/8, two on board (addr D0 and D8)
 
         command bits: RCCOSSGG
         R = "Ready Bit," initiates new conversion in one-shot mode
                          resets to 1 when new conversion is settled
         CC = Channel Selection
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.19.0/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/project_controller.py` & `naludaq-0.19.0/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.19.0/src/naludaq/controllers/readout/trbhm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-"""Readout settings for the aardvarcv3 board.
-
-When setting the readout channel, aardvarc uses exclude channel mask registers
-to exclude certain channels from readout
+"""Readout settings for the board.
 
 Controls the readout channels and the readout windows.
 """
 from logging import getLogger
 
 from .default import ReadoutController
 
-LOGGER = getLogger("naludaq.readout_controller_aardvarcv3")
+LOGGER = getLogger("naludaq.readout_controller_default")
+MAX_READOUT = 65536
+
+
+class TrbhmReadoutController(ReadoutController):
+    """Special readout controller for the TRHBM.
 
+    Overrides the channel-setting logic.
+    """
 
-class Aardvarcv3ReadoutController(ReadoutController):
     def __init__(self, board):
-        """Readout Controller for aardvarcv3.
-        Args:
-            board (Board): the board object.
-        """
         super().__init__(board)
 
     def set_readout_channels(self, channels_to_read: list):
         """Select channels to readout.
 
-        Update the registers and write them to the board.
+        TRBHM currently doesn't support setting channels individually
+        across both ASICs; their 'chansel' is shared.
 
         Args:
             channels_to_read(list): List of channel numbers to read
-
-        Raises:
-            TypeError if the list or an element in the list are the wrong type
-            ValueError if the list is too large, too small, or contains a channel
-                number that is out of bounds.
-
+                Accepts channels 1..8 for consistent API, but does
+                a logical OR between the upper and lower 4 channels.
         """
         self._validate_channels_or_raise(channels_to_read)
-        chansel = self._generate_channels_bits(channels_to_read)
-        max_chan = self.board.params["channels"]
-        # Exclude channel mask is opposite of chansel
-        excludechanmask = (2**max_chan - 1) ^ int(chansel, 2)
-        self._write_digital_register("excludechannelmask", excludechanmask)
 
-    def get_readout_channels(self):
-        """Get the current channels to read out.
-
-        Returns:
-            Sorted list of channel numbers to read out.
-        """
-        mask = self.board.registers["digital_registers"]["excludechannelmask"]["value"][
-            0
-        ]
-        return [c for c in range(self.board.channels) if (mask >> c) & 1 == 0]
+        chansel_lower = sum([1 << x for x in channels_to_read if x < 4])
+        chansel_upper = sum([1 << (x - 4) for x in channels_to_read if x >= 4])
+        self._write_control_register("chansel", chansel_lower | chansel_upper)
+
+    def get_readout_channels(self) -> "list[int]":
+        """Get the enabled readout channels as a list[int]."""
+        chansel = self.board.registers["control_registers"]["chansel"]["value"]
+        chansel = f"{chansel:02b}"
+        return [c for c in range(self.board.channels) if chansel[c % 4] == "1"]
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/readout/default.py` & `naludaq-0.19.0/src/naludaq/controllers/readout/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,22 +341,27 @@
         chansel = self.board.registers["control_registers"]["chansel"]
         return [
             (x)
             for x, val in enumerate(reversed(list(bin(chansel["value"])[2:])))
             if int(val) == 1
         ]
 
-    def _write_analog_register(self, register: str, value: int):
+    def _write_analog_register(
+        self,
+        register: str,
+        value: int,
+        chips: "int | list[int] | None" = None,
+    ):
         """Helper function for writing analog registers.
 
         Args:
             register (str): register name
             value (int): value to write.
         """
-        AnalogRegisters(self.board).write(register, value)
+        AnalogRegisters(self.board, chips).write(register, value)
 
     def _write_control_register(self, register: str, value: int):
         """Helper function for writing control registers.
 
         Args:
             register (str): register name
             value (int): value to write.
```

### Comparing `naludaq-0.18.0/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.19.0/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/tia/base.py` & `naludaq-0.19.0/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/default.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.19.0/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/__init__.py` & `naludaq-0.19.0/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/debugdaq.py` & `naludaq-0.19.0/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/lightdaq.py` & `naludaq-0.19.0/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/preprocess.py` & `naludaq-0.19.0/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/__init__.py` & `naludaq-0.19.0/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.19.0/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.19.0/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.19.0/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.19.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.19.0/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.19.0/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.19.0/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.19.0/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/devices/eeprom.py` & `naludaq-0.19.0/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/devices/i2c_device.py` & `naludaq-0.19.0/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/devices/ltc2990.py` & `naludaq-0.19.0/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/helpers/decorators.py` & `naludaq-0.19.0/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/helpers/exceptions.py` & `naludaq-0.19.0/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/helpers/helper_functions.py` & `naludaq-0.19.0/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/helpers/register_cache.py` & `naludaq-0.19.0/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/helpers/semiton.py` & `naludaq-0.19.0/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/helpers/validations.py` & `naludaq-0.19.0/src/naludaq/helpers/validations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/io/__init__.py` & `naludaq-0.19.0/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/io/csv_writer.py` & `naludaq-0.19.0/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/io/hdf5.py` & `naludaq-0.19.0/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/io/io_manager.py` & `naludaq-0.19.0/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/models/acq_converters.py` & `naludaq-0.19.0/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/models/acquisition.py` & `naludaq-0.19.0/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/naludaq.py` & `naludaq-0.19.0/src/naludaq/naludaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/__init__.py` & `naludaq-0.19.0/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/answer_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/base.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/siread.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.19.0/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/parser.py` & `naludaq-0.19.0/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/udc_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/parsers/upac_parser.py` & `naludaq-0.19.0/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.19.0/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.19.0/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.19.0/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/autoaction.py` & `naludaq-0.19.0/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.19.0/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/board_backup.py` & `naludaq-0.19.0/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.19.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/data_collector.py` & `naludaq-0.19.0/src/naludaq/tools/data_collector.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/features.py` & `naludaq-0.19.0/src/naludaq/tools/features.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,43 @@
 
 _FEATURES = {
     "adc2mv": Feature(
         description="ADC to mV Calibration",
         long_description="Allows calibration to convert from units of ADC to mV",
         beta_models=get_available_models(),
     ),
+    "calibration_channel": Feature(
+        description="Calibration Channel",
+        long_description=(
+            "Allows control of the calibration channel on the board. "
+            "Other channels on the board may be swapped with the calibration channel."
+        ),
+        beta_models=[],
+    ),
     "dac_sweep": Feature(
         description="External DAC Sweep",
         long_description=(
             "Gathers data at various DAC values to characterize the response to "
             "different input levels"
         ),
         beta_models=get_available_models(),
     ),
     "ext_dac": Feature(
         description="External DAC",
         long_description="Allows control of the external DAC on the board",
         beta_models=[],
     ),
+    "gain_stage_tuner": Feature(
+        description="Gain Stage Tuner",
+        long_description=(
+            "Calibrates external dac and ISEL for a specific "
+            "gain stage configuration"
+        ),
+        beta_models=get_available_models(),
+    ),
     "pedestals": Feature(
         description="Pedestal Calibration",
         long_description="Allows generation of pedestals data and subtraction of built-in noise",
         beta_models=[],
     ),
     "threshold_scan": Feature(
         description="Threshold Scan",
@@ -59,22 +75,14 @@
         description="Timing Calibration",
         long_description=(
             "Enables calibration of the internal timing circuit "
             "for better sample-to-sample timing precision"
         ),
         beta_models=get_available_models(),
     ),
-    "gain_stage_tuner": Feature(
-        description="Gain Stage Tuner",
-        long_description=(
-            "Calibrates external dac and ISEL for a specific "
-            "gain stage configuration"
-        ),
-        beta_models=get_available_models(),
-    ),
 }
 
 
 def features_names() -> list[str]:
     """Get a list of available feature names"""
     return list(_FEATURES.keys())
```

### Comparing `naludaq-0.18.0/src/naludaq/tools/ft60x.py` & `naludaq-0.19.0/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/ftdi.py` & `naludaq-0.19.0/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/metadata.py` & `naludaq-0.19.0/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.19.0/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.19.0/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/__init__.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/aav3.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/aav3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/default.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/_new/hdsoc.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/_new/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_acq.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_acq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_controller.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/udc16_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py` & `naludaq-0.19.0/src/naludaq/tools/pedestals/upac96_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.19.0/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.19.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.19.0/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.19.0/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.19.0/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.19.0/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.19.0/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.18.0/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.19.0/src/naludaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.18.0
+Version: 0.19.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -82,15 +82,15 @@
 
 ```
 pip install -e .[dev]
 ```
 
 The package can now be imported in your project and edited in your favorite editor, [VS Code](https://code.visualstudio.com/)
 
-## Development wtih gigabit ethernet backend
+## Development with gigabit ethernet backend
 
 To use the gigabit ethernet backend you will need to install the `naludaq_rs` package.
 
 1. Clone the package from GitHub
 2. install the package as an editable package. See instructions in the `naludaq_rs` package.
 
 
@@ -104,14 +104,18 @@
 pre-commit install
 ```
 
 The hooks will run automatically when you commit changes to the repository.
 
 The code MUST run the pre-commit hooks before commiting. If the hooks fail, the commit will be rejected.
 
+# Examples
+
+See the [example repository](https://github.com/NaluScientific/naluexamples).
+
 # Development Use
 
 Once the package is installed it's now possible to start using the package.
 There is a boilerplate interface named `Naludaq` in `naludaq` it contains basic functionality.
 It's a good starting point to get the software started.
 If more advanced scripts are required please continue reading below.
 A datasheet for the board is also required to understand the registers and the commands.
```

### Comparing `naludaq-0.18.0/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.19.0/src/naludaq.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,26 +61,28 @@
 src/naludaq/controllers/controller.py
 src/naludaq/controllers/project_controller.py
 src/naludaq/controllers/si5341_controller.py
 src/naludaq/controllers/biasing_mode/__init__.py
 src/naludaq/controllers/biasing_mode/udc16.py
 src/naludaq/controllers/board/__init__.py
 src/naludaq/controllers/board/aodsoc.py
+src/naludaq/controllers/board/asocv3.py
 src/naludaq/controllers/board/default.py
 src/naludaq/controllers/board/hdsoc.py
 src/naludaq/controllers/board/oleas.py
 src/naludaq/controllers/board/trbhm.py
 src/naludaq/controllers/board/udc.py
 src/naludaq/controllers/board/upac.py
 src/naludaq/controllers/board/upac96.py
 src/naludaq/controllers/connection/__init__.py
 src/naludaq/controllers/connection/connection_controller.py
 src/naludaq/controllers/connection/upac.py
 src/naludaq/controllers/connection/upac96.py
 src/naludaq/controllers/external_dac/__init__.py
+src/naludaq/controllers/external_dac/aardvarcv3.py
 src/naludaq/controllers/external_dac/ad5671.py
 src/naludaq/controllers/external_dac/ad5675.py
 src/naludaq/controllers/external_dac/base.py
 src/naludaq/controllers/external_dac/dac7578.py
 src/naludaq/controllers/external_dac/hdsoc.py
 src/naludaq/controllers/external_dac/i2c_dac.py
 src/naludaq/controllers/external_dac/trbhm.py
@@ -176,14 +178,17 @@
 src/naludaq/tools/adc2mv/adc_linear_regression.py
 src/naludaq/tools/adc2mv/generate.py
 src/naludaq/tools/adc2mv/pre_adc2mv.py
 src/naludaq/tools/autotrigger/__init__.py
 src/naludaq/tools/autotrigger/default.py
 src/naludaq/tools/dac_sweep/__init__.py
 src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+src/naludaq/tools/lookup_table/__init__.py
+src/naludaq/tools/lookup_table/lookup_table.py
+src/naludaq/tools/lookup_table/lookup_table_generator.py
 src/naludaq/tools/optimizers/__init__.py
 src/naludaq/tools/optimizers/bayesian_optimizer.py
 src/naludaq/tools/optimizers/gainstagetuner.py
 src/naludaq/tools/pedestals/__init__.py
 src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
 src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
 src/naludaq/tools/pedestals/pedestals_acq.py
```

