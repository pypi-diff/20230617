# Comparing `tmp/ecowitt2mqtt-2023.5.0.tar.gz` & `tmp/ecowitt2mqtt-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecowitt2mqtt-2023.5.0.tar", max compression
+gzip compressed data, was "ecowitt2mqtt-2023.6.0.tar", max compression
```

## Comparing `ecowitt2mqtt-2023.5.0.tar` & `ecowitt2mqtt-2023.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/LICENSE
--rw-r--r--   0        0        0    31131 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/README.md
--rw-r--r--   0        0        0       39 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/__init__.py
--rw-r--r--   0        0        0    13841 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/__main__.py
--rw-r--r--   0        0        0       24 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/backports/__init__.py
--rw-r--r--   0        0        0     1735 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/backports/enum.py
--rw-r--r--   0        0        0    16656 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/config.py
--rw-r--r--   0        0        0    11058 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/const.py
--rw-r--r--   0        0        0     2308 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/core.py
--rw-r--r--   0        0        0    11872 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/data.py
--rw-r--r--   0        0        0      107 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/errors.py
--rw-r--r--   0        0        0       22 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/__init__.py
--rw-r--r--   0        0        0     6598 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/__init__.py
--rw-r--r--   0        0        0     4891 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/battery.py
--rw-r--r--   0        0        0     2301 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/humidity.py
--rw-r--r--   0        0        0     2438 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/illuminance.py
--rw-r--r--   0        0        0     1018 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/leak.py
--rw-r--r--   0        0        0     2013 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/lightning.py
--rw-r--r--   0        0        0      744 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pollution.py
--rw-r--r--   0        0        0     2737 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/precipitation.py
--rw-r--r--   0        0        0     1364 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pressure.py
--rw-r--r--   0        0        0    21443 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/temperature.py
--rw-r--r--   0        0        0     1333 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/time.py
--rw-r--r--   0        0        0     4610 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/uv.py
--rw-r--r--   0        0        0     9593 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/wind.py
--rw-r--r--   0        0        0     2167 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/config_validation.py
--rw-r--r--   0        0        0     1619 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/device.py
--rw-r--r--   0        0        0     1800 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/__init__.py
--rw-r--r--   0        0        0      716 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/factory.py
--rw-r--r--   0        0        0    18180 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/hass.py
--rw-r--r--   0        0        0     1114 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/topic.py
--rw-r--r--   0        0        0     4973 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/server.py
--rw-r--r--   0        0        0      348 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/typing.py
--rw-r--r--   0        0        0     7978 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/runtime.py
--rw-r--r--   0        0        0     1255 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/__init__.py
--rw-r--r--   0        0        0     7934 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/meteo.py
--rw-r--r--   0        0        0    13191 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/unit_conversion.py
--rw-r--r--   0        0        0     4055 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/pyproject.toml
--rw-r--r--   0        0        0    32763 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/LICENSE
+-rw-r--r--   0        0        0    31131 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/README.md
+-rw-r--r--   0        0        0       39 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/__init__.py
+-rw-r--r--   0        0        0    13841 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/__main__.py
+-rw-r--r--   0        0        0       24 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/backports/__init__.py
+-rw-r--r--   0        0        0     1735 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/backports/enum.py
+-rw-r--r--   0        0        0    16441 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/config.py
+-rw-r--r--   0        0        0    10920 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/const.py
+-rw-r--r--   0        0        0     2308 2023-06-17 17:57:01.588773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/core.py
+-rw-r--r--   0        0        0    12177 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/data.py
+-rw-r--r--   0        0        0      107 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/errors.py
+-rw-r--r--   0        0        0       22 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/__init__.py
+-rw-r--r--   0        0        0     6598 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/__init__.py
+-rw-r--r--   0        0        0     4891 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/battery.py
+-rw-r--r--   0        0        0     2301 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/humidity.py
+-rw-r--r--   0        0        0     2438 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/illuminance.py
+-rw-r--r--   0        0        0     1018 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/leak.py
+-rw-r--r--   0        0        0     2013 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/lightning.py
+-rw-r--r--   0        0        0      744 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pollution.py
+-rw-r--r--   0        0        0     2737 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/precipitation.py
+-rw-r--r--   0        0        0     1364 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pressure.py
+-rw-r--r--   0        0        0    21443 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/temperature.py
+-rw-r--r--   0        0        0     1639 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/time.py
+-rw-r--r--   0        0        0     4610 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/uv.py
+-rw-r--r--   0        0        0     9593 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/wind.py
+-rw-r--r--   0        0        0     2167 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/config_validation.py
+-rw-r--r--   0        0        0     1665 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/device.py
+-rw-r--r--   0        0        0     1800 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/factory.py
+-rw-r--r--   0        0        0    18157 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/hass.py
+-rw-r--r--   0        0        0     1114 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/topic.py
+-rw-r--r--   0        0        0     4973 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/server.py
+-rw-r--r--   0        0        0      348 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/typing.py
+-rw-r--r--   0        0        0     8058 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/runtime.py
+-rw-r--r--   0        0        0     1414 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/__init__.py
+-rw-r--r--   0        0        0     7934 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/meteo.py
+-rw-r--r--   0        0        0    13191 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/unit_conversion.py
+-rw-r--r--   0        0        0     4077 2023-06-17 17:57:01.592773 ecowitt2mqtt-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0    32563 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.6.0/PKG-INFO
```

### Comparing `ecowitt2mqtt-2023.5.0/LICENSE` & `ecowitt2mqtt-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/README.md` & `ecowitt2mqtt-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/__main__.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/backports/enum.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/backports/enum.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/config.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Define a configuration management module."""
 from __future__ import annotations
 
 import os
 from collections.abc import Generator
 from typing import Any, cast
+from uuid import uuid4
 
 import voluptuous as vol
 from ruamel.yaml import YAML
 
 import ecowitt2mqtt.helpers.config_validation as cv
 from ecowitt2mqtt.const import (
     CONF_BATTERY_OVERRIDES,
@@ -76,15 +77,14 @@
     },
     extra=vol.ALLOW_EXTRA,
 )
 
 MQTT_TOPIC_SCHEMA = vol.Schema(
     {
         vol.Required(CONF_MQTT_TOPIC): str,
-        vol.Optional(CONF_HASS_DISCOVERY, default=False): vol.All(cv.boolean, False),
     },
     extra=vol.ALLOW_EXTRA,
 )
 
 CONFIG_SCHEMA = vol.All(
     vol.Any(
         HASS_DISCOVERY_SCHEMA,
@@ -199,18 +199,15 @@
             self._config[CONF_BATTERY_OVERRIDES] = battery_overrides_env_var
 
         try:
             self._config = CONFIG_SCHEMA(self._config)
         except vol.Invalid as err:
             raise ConfigError(err) from err
 
-        self._mqtt_connection_info = (
-            f"{self._config.get(CONF_MQTT_USERNAME)}@{self._config[CONF_MQTT_BROKER]}"
-            f":{self._config[CONF_MQTT_PORT]}"
-        )
+        self._uuid = uuid4().hex
 
     def __repr__(self) -> str:
         """Define a string representation of this object.
 
         Returns:
             A string representation.
         """
@@ -312,21 +309,21 @@
 
         Returns:
             The MQTT broker info string.
         """
         return cast(str, self._config[CONF_MQTT_BROKER])
 
     @property
-    def mqtt_connection_info(self) -> str:
-        """Return a string representation of MQTT connection parameters.
+    def uuid(self) -> str:
+        """Return the unique ID of this Config object.
 
         Returns:
             The connection info string.
         """
-        return self._mqtt_connection_info
+        return self._uuid
 
     @property
     def mqtt_password(self) -> str | None:
         """Return the MQTT broker password.
 
         Returns:
             The MQTT password string.
@@ -510,20 +507,21 @@
 
         if config_path := config.get(CONF_CONFIG):
             config_file_config = load_config_from_file(config_path)
         else:
             config_file_config = {}
 
         # Store the default config:
-        self._configs[CONF_DEFAULT] = Config(config_file_config | config)
+        default_config = config | config_file_config
+        self._configs[CONF_DEFAULT] = Config(default_config)
 
         # Store configs for any gateways:
         gateways_file_config = config_file_config.get(CONF_GATEWAYS, {})
         for passkey, gateway_config in gateways_file_config.items():
-            self._configs[passkey] = Config(gateway_config | config)
+            self._configs[passkey] = Config(default_config | gateway_config)
 
     def __repr__(self) -> str:
         """Define a string representation of this object.
 
         Returns:
             A string representation.
         """
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/const.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define package constants."""
 import logging
 from typing import Final
 
 from ecowitt2mqtt.helpers.typing import UnitSystemType
 
-__version__ = "2023.05.0"
+__version__ = "2023.06.0"
 
 LOGGER = logging.getLogger(__package__)
 
 # Configuration keys:
 CONF_BATTERY_OVERRIDES: Final = "battery_override"
 CONF_CONFIG: Final = "config"
 CONF_DEFAULT_BATTERY_STRATEGY: Final = "default_battery_strategy"
@@ -43,24 +43,26 @@
 CONF_PRECISION: Final = "precision"
 CONF_RAW_DATA: Final = "raw_data"
 CONF_VERBOSE: Final = "verbose"
 
 # Data points (glob):
 DATA_POINT_GLOB_BAROM: Final = "barom"
 DATA_POINT_GLOB_BATT: Final = "batt"
+DATA_POINT_GLOB_GAIN_PIEZO: Final = "gain_piezo"
 DATA_POINT_GLOB_GUST: Final = "gust"
 DATA_POINT_GLOB_HUMIDITY: Final = "humidity"
 DATA_POINT_GLOB_LEAFBATT: Final = "leaf_batt"
 DATA_POINT_GLOB_LEAK: Final = "leak"
 DATA_POINT_GLOB_LEAKBATT: Final = "leakbatt"
 DATA_POINT_GLOB_MOISTURE: Final = "moisture"
 DATA_POINT_GLOB_PM10: Final = "pm10"
 DATA_POINT_GLOB_PM25: Final = "pm25"
 DATA_POINT_GLOB_PM25BATT: Final = "pm25batt"
 DATA_POINT_GLOB_RAIN: Final = "rain"
+DATA_POINT_GLOB_RAIN_PIEZO: Final = "rain_piezo"
 DATA_POINT_GLOB_R_RAIN: Final = "rrain"
 DATA_POINT_GLOB_SOILBATT: Final = "soilbatt"
 DATA_POINT_GLOB_TEMP: Final = "temp"
 DATA_POINT_GLOB_TF: Final = "tf"
 DATA_POINT_GLOB_TF_BATT: Final = "tf_batt"
 DATA_POINT_GLOB_VOLT: Final = "volt"
 DATA_POINT_GLOB_WETNESS: Final = "wetness"
@@ -70,34 +72,31 @@
 # Data points (specific):
 DATA_POINT_BEAUFORT_SCALE: Final = "beaufortscale"
 DATA_POINT_CO2: Final = "co2"
 DATA_POINT_CO2_24H: Final = "co2_24h"
 DATA_POINT_CO2_BATT: Final = "co2_batt"
 DATA_POINT_DAILY_RAIN: Final = "dailyrain"
 DATA_POINT_DEWPOINT: Final = "dewpoint"
-DATA_POINT_DRAIN_PIEZO: Final = "drain_piezo"
-DATA_POINT_ERAIN_PIEZO: Final = "erain_piezo"
 DATA_POINT_EVENT_RAIN: Final = "eventrain"
 DATA_POINT_FEELSLIKE: Final = "feelslike"
 DATA_POINT_FROST_POINT: Final = "frostpoint"
 DATA_POINT_FROST_RISK: Final = "frostrisk"
 DATA_POINT_HEATINDEX: Final = "heatindex"
 DATA_POINT_HOURLY_RAIN: Final = "hourlyrain"
-DATA_POINT_HRAIN_PIEZO: Final = "hrain_piezo"
 DATA_POINT_HUMIDEX: Final = "humidex"
 DATA_POINT_HUMIDEX_PERCEPTION: Final = "humidex_perception"
 DATA_POINT_HUMIDITY: Final = "humidity"
 DATA_POINT_HUMIDITY_ABS: Final = "humidityabs"
 DATA_POINT_HUMIDITY_ABS_IN: Final = "humidityabsin"
 DATA_POINT_HUMI_CO2: Final = "humi_co2"
+DATA_POINT_INTERVAL: Final = "interval"
 DATA_POINT_LIGHTNING: Final = "lightning"
 DATA_POINT_LIGHTNING_NUM: Final = "lightning_num"
 DATA_POINT_LIGHTNING_TIME: Final = "lightning_time"
 DATA_POINT_MONTHLY_RAIN: Final = "monthlyrain"
-DATA_POINT_MRAIN_PIEZO: Final = "mrain_piezo"
 DATA_POINT_RAIN_RATE: Final = "rainrate"
 DATA_POINT_RELATIVE_STRAIN_INDEX: Final = "relative_strain_index"
 DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION: Final = "relative_strain_index_perception"
 DATA_POINT_RUNTIME: Final = "runtime"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1: Final = "safe_exposure_time_skin_type_1"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2: Final = "safe_exposure_time_skin_type_2"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_3: Final = "safe_exposure_time_skin_type_3"
@@ -122,18 +121,16 @@
 DATA_POINT_WH68BATT: Final = "wh68batt"
 DATA_POINT_WH80BATT: Final = "wh80batt"
 DATA_POINT_WH90BATT: Final = "wh90batt"
 DATA_POINT_WH90BATT_PC: Final = "wh90battpc"
 DATA_POINT_WH90CAP_VOLT: Final = "ws90cap_volt"
 DATA_POINT_WINDCHILL: Final = "windchill"
 DATA_POINT_WINDSPEED: Final = "windspeed"
-DATA_POINT_WRAIN_PIEZO: Final = "wrain_piezo"
 DATA_POINT_WS90_VER: Final = "ws90_ver"
 DATA_POINT_YEARLY_RAIN: Final = "yearlyrain"
-DATA_POINT_YRAIN_PIEZO: Final = "yrain_piezo"
 
 # Defaults:
 DEFAULT_ENDPOINT: Final = "/data/report"
 DEFAULT_HASS_DISCOVERY_PREFIX: Final = "homeassistant"
 DEFAULT_MQTT_PORT: Final = 1883
 DEFAULT_PORT: Final = 8080
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/core.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/core.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/data.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,38 @@
     DATA_POINT_CO2_24H,
     DATA_POINT_DEWPOINT,
     DATA_POINT_FEELSLIKE,
     DATA_POINT_FROST_POINT,
     DATA_POINT_FROST_RISK,
     DATA_POINT_GLOB_BAROM,
     DATA_POINT_GLOB_BATT,
+    DATA_POINT_GLOB_GAIN_PIEZO,
     DATA_POINT_GLOB_GUST,
     DATA_POINT_GLOB_HUMIDITY,
     DATA_POINT_GLOB_LEAK,
     DATA_POINT_GLOB_MOISTURE,
     DATA_POINT_GLOB_PM10,
     DATA_POINT_GLOB_PM25,
     DATA_POINT_GLOB_R_RAIN,
     DATA_POINT_GLOB_RAIN,
+    DATA_POINT_GLOB_RAIN_PIEZO,
     DATA_POINT_GLOB_TEMP,
     DATA_POINT_GLOB_TF,
     DATA_POINT_GLOB_VOLT,
     DATA_POINT_GLOB_WETNESS,
     DATA_POINT_GLOB_WIND,
     DATA_POINT_GLOB_WINDDIR,
     DATA_POINT_HEATINDEX,
     DATA_POINT_HUMI_CO2,
     DATA_POINT_HUMIDEX,
     DATA_POINT_HUMIDEX_PERCEPTION,
     DATA_POINT_HUMIDITY,
     DATA_POINT_HUMIDITY_ABS,
     DATA_POINT_HUMIDITY_ABS_IN,
+    DATA_POINT_INTERVAL,
     DATA_POINT_LIGHTNING,
     DATA_POINT_LIGHTNING_NUM,
     DATA_POINT_LIGHTNING_TIME,
     DATA_POINT_RAIN_RATE,
     DATA_POINT_RELATIVE_STRAIN_INDEX,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION,
     DATA_POINT_RUNTIME,
@@ -60,14 +63,15 @@
     LOGGER,
 )
 from ecowitt2mqtt.helpers.calculator import (
     CalculatedDataPoint,
     CalculationFailedError,
     CalculationKeysMissingError,
     Calculator,
+    SimpleCalculator,
 )
 from ecowitt2mqtt.helpers.calculator.battery import BatteryCalculator
 from ecowitt2mqtt.helpers.calculator.humidity import (
     AbsoluteHumidityCalculator,
     RelativeHumidityCalculator,
 )
 from ecowitt2mqtt.helpers.calculator.illuminance import (
@@ -97,15 +101,19 @@
     RsiPerceptionCalculator,
     SimmerIndexCalculator,
     SimmerZoneCalculator,
     TemperatureCalculator,
     ThermalPerceptionCalculator,
     WindChillCalculator,
 )
-from ecowitt2mqtt.helpers.calculator.time import EpochCalculator, RuntimeCalculator
+from ecowitt2mqtt.helpers.calculator.time import (
+    EpochCalculator,
+    RuntimeCalculator,
+    UpdateIntervalCalculator,
+)
 from ecowitt2mqtt.helpers.calculator.uv import SafeExposureCalculator, UVIndexCalculator
 from ecowitt2mqtt.helpers.calculator.wind import (
     BeaufortScaleCalculator,
     WindDirCalculator,
     WindSpeedCalculator,
 )
 from ecowitt2mqtt.helpers.device import Device, get_device_from_raw_payload
@@ -118,35 +126,38 @@
     DATA_POINT_CO2_24H: PollutantCalculator,
     DATA_POINT_DEWPOINT: DewPointCalculator,
     DATA_POINT_FEELSLIKE: FeelsLikeCalculator,
     DATA_POINT_FROST_POINT: FrostPointCalculator,
     DATA_POINT_FROST_RISK: FrostRiskCalculator,
     DATA_POINT_GLOB_BAROM: PressureCalculator,
     DATA_POINT_GLOB_BATT: BatteryCalculator,
+    DATA_POINT_GLOB_GAIN_PIEZO: SimpleCalculator,
     DATA_POINT_GLOB_GUST: WindSpeedCalculator,
     DATA_POINT_GLOB_HUMIDITY: RelativeHumidityCalculator,
     DATA_POINT_GLOB_LEAK: LeakCalculator,
     DATA_POINT_GLOB_MOISTURE: RelativeHumidityCalculator,
     DATA_POINT_GLOB_PM10: PollutantCalculator,
     DATA_POINT_GLOB_PM25: PollutantCalculator,
     DATA_POINT_GLOB_RAIN: AccumulatedPrecipitationCalculator,
+    DATA_POINT_GLOB_RAIN_PIEZO: SimpleCalculator,
     DATA_POINT_GLOB_R_RAIN: PrecipitationRateCalculator,
     DATA_POINT_GLOB_TEMP: TemperatureCalculator,
     DATA_POINT_GLOB_TF: TemperatureCalculator,
     DATA_POINT_GLOB_VOLT: BatteryCalculator,
     DATA_POINT_GLOB_WETNESS: RelativeHumidityCalculator,
     DATA_POINT_GLOB_WIND: WindSpeedCalculator,
     DATA_POINT_GLOB_WINDDIR: WindDirCalculator,
     DATA_POINT_HEATINDEX: HeatIndexCalculator,
     DATA_POINT_HUMIDEX: HumidexCalculator,
     DATA_POINT_HUMIDEX_PERCEPTION: HumidexPerceptionCalculator,
     DATA_POINT_HUMIDITY: RelativeHumidityCalculator,
     DATA_POINT_HUMIDITY_ABS: AbsoluteHumidityCalculator,
     DATA_POINT_HUMIDITY_ABS_IN: AbsoluteHumidityCalculator,
     DATA_POINT_HUMI_CO2: RelativeHumidityCalculator,
+    DATA_POINT_INTERVAL: UpdateIntervalCalculator,
     DATA_POINT_LIGHTNING: LightningStrikeDistanceCalculator,
     DATA_POINT_LIGHTNING_NUM: LightningStrikeCountCalculator,
     DATA_POINT_LIGHTNING_TIME: EpochCalculator,
     DATA_POINT_RAIN_RATE: PrecipitationRateCalculator,
     DATA_POINT_RELATIVE_STRAIN_INDEX: RsiCalculator,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION: RsiPerceptionCalculator,
     DATA_POINT_RUNTIME: RuntimeCalculator,
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/__init__.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/battery.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/battery.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/humidity.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/humidity.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/illuminance.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/illuminance.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/leak.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/leak.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/lightning.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/lightning.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pollution.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pollution.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/precipitation.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/precipitation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pressure.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/pressure.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/temperature.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/temperature.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/time.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/time.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,7 +44,20 @@
     def output_unit(self) -> str:
         """Get the output unit of measurement for this calculation.
 
         Returns:
             A unit string.
         """
         return TIME_SECONDS
+
+
+class UpdateIntervalCalculator(SimpleCalculator):
+    """Define a data update interval calculator."""
+
+    @property
+    def output_unit(self) -> str:
+        """Get the output unit of measurement for this calculation.
+
+        Returns:
+            A unit string.
+        """
+        return TIME_SECONDS
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/uv.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/uv.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/wind.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/calculator/wind.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/config_validation.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/config_validation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/device.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 DEFAULT_MODEL = "Unknown Model"
 DEFAULT_NAME = "Unknown Device"
 
 MODEL_BRAND_MAP = {
     "GW1000": "Ecowitt",
     "GW1100": "Ecowitt",
     "GW2000": "Ecowitt",
-    "HP2550": "Fine Offset",
+    "HP2550": "Ecowitt",
     "HP2551": "Ecowitt",
+    "HP2553": "Ecowitt",
+    "HP2564": "Ecowitt",
     "PT-HP2550": "Fine Offset",
     "WH2650": "Fine Offset",
     "WS2350": "La Crosse",
     "WS2900": "Ambient Weather",
 }
 
 STATION_TYPE_BRAND_MAP = {
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/__init__.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/factory.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.helpers.publisher import MqttPublisher
 from ecowitt2mqtt.helpers.publisher.hass import HomeAssistantDiscoveryPublisher
 from ecowitt2mqtt.helpers.publisher.topic import TopicPublisher
 
 
-def get_publisher(config: Config, client: Client) -> MqttPublisher:
-    """Get an MQTT publisher.
+def get_publishers(config: Config, client: Client) -> list[MqttPublisher]:
+    """Get configured MQTT publishers.
 
     Args:
         config: A Config object.
         client: An MQTT Client object.
 
     Returns:
-        An MqttPublisher object.
+        A list of MqttPublisher objects.
     """
+    publishers: list[MqttPublisher] = []
     if config.hass_discovery:
-        return HomeAssistantDiscoveryPublisher(config, client)
-    return TopicPublisher(config, client)
+        publishers.append(HomeAssistantDiscoveryPublisher(config, client))
+    if config.mqtt_topic:
+        publishers.append(TopicPublisher(config, client))
+    return publishers
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/hass.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/hass.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,49 +12,48 @@
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.const import (
     DATA_POINT_BEAUFORT_SCALE,
     DATA_POINT_CO2,
     DATA_POINT_CO2_24H,
     DATA_POINT_DAILY_RAIN,
     DATA_POINT_DEWPOINT,
-    DATA_POINT_DRAIN_PIEZO,
-    DATA_POINT_ERAIN_PIEZO,
     DATA_POINT_EVENT_RAIN,
     DATA_POINT_FEELSLIKE,
     DATA_POINT_FROST_POINT,
     DATA_POINT_FROST_RISK,
     DATA_POINT_GLOB_BAROM,
     DATA_POINT_GLOB_BATT,
+    DATA_POINT_GLOB_GAIN_PIEZO,
     DATA_POINT_GLOB_GUST,
     DATA_POINT_GLOB_HUMIDITY,
     DATA_POINT_GLOB_LEAK,
     DATA_POINT_GLOB_MOISTURE,
     DATA_POINT_GLOB_PM10,
     DATA_POINT_GLOB_PM25,
     DATA_POINT_GLOB_R_RAIN,
     DATA_POINT_GLOB_RAIN,
+    DATA_POINT_GLOB_RAIN_PIEZO,
     DATA_POINT_GLOB_TEMP,
     DATA_POINT_GLOB_TF,
     DATA_POINT_GLOB_VOLT,
     DATA_POINT_GLOB_WETNESS,
     DATA_POINT_GLOB_WIND,
     DATA_POINT_GLOB_WINDDIR,
     DATA_POINT_HEATINDEX,
     DATA_POINT_HOURLY_RAIN,
-    DATA_POINT_HRAIN_PIEZO,
     DATA_POINT_HUMI_CO2,
     DATA_POINT_HUMIDEX,
     DATA_POINT_HUMIDEX_PERCEPTION,
     DATA_POINT_HUMIDITY_ABS,
     DATA_POINT_HUMIDITY_ABS_IN,
+    DATA_POINT_INTERVAL,
     DATA_POINT_LIGHTNING,
     DATA_POINT_LIGHTNING_NUM,
     DATA_POINT_LIGHTNING_TIME,
     DATA_POINT_MONTHLY_RAIN,
-    DATA_POINT_MRAIN_PIEZO,
     DATA_POINT_RAIN_RATE,
     DATA_POINT_RELATIVE_STRAIN_INDEX,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION,
     DATA_POINT_RUNTIME,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_3,
@@ -67,18 +66,16 @@
     DATA_POINT_SOLARRADIATION_PERCEIVED,
     DATA_POINT_TF_CO2,
     DATA_POINT_THERMAL_PERCEPTION,
     DATA_POINT_TOTAL_RAIN,
     DATA_POINT_UV,
     DATA_POINT_WEEKLY_RAIN,
     DATA_POINT_WINDCHILL,
-    DATA_POINT_WRAIN_PIEZO,
     DATA_POINT_WS90_VER,
     DATA_POINT_YEARLY_RAIN,
-    DATA_POINT_YRAIN_PIEZO,
     LOGGER,
 )
 from ecowitt2mqtt.data import ProcessedData
 from ecowitt2mqtt.helpers.calculator import CalculatedDataPoint, DataPointType
 from ecowitt2mqtt.helpers.calculator.battery import (
     BatteryStrategy,
     get_battery_strategy,
@@ -205,14 +202,17 @@
     DATA_POINT_FROST_RISK: EntityDescription(
         icon="mdi:snowflake-alert",
     ),
     DATA_POINT_GLOB_BAROM: EntityDescription(
         device_class=DeviceClass.PRESSURE,
         state_class=StateClass.MEASUREMENT,
     ),
+    DATA_POINT_GLOB_GAIN_PIEZO: EntityDescription(
+        entity_category=EntityCategory.DIAGNOSTIC,
+    ),
     DATA_POINT_GLOB_GUST: EntityDescription(
         icon="mdi:weather-windy",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_HUMIDITY: EntityDescription(
         device_class=DeviceClass.HUMIDITY,
         state_class=StateClass.MEASUREMENT,
@@ -237,14 +237,17 @@
         icon="mdi:water",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_RAIN: EntityDescription(
         icon="mdi:water",
         state_class=StateClass.MEASUREMENT,
     ),
+    DATA_POINT_GLOB_RAIN_PIEZO: EntityDescription(
+        entity_category=EntityCategory.DIAGNOSTIC,
+    ),
     DATA_POINT_GLOB_TEMP: EntityDescription(
         device_class=DeviceClass.TEMPERATURE,
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_GLOB_TF: EntityDescription(
         device_class=DeviceClass.TEMPERATURE,
         state_class=StateClass.MEASUREMENT,
@@ -283,14 +286,18 @@
         icon="mdi:water-percent",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_HUMIDITY_ABS_IN: EntityDescription(
         icon="mdi:water-percent",
         state_class=StateClass.MEASUREMENT,
     ),
+    DATA_POINT_INTERVAL: EntityDescription(
+        icon="mdi:water-percent",
+        entity_category=EntityCategory.DIAGNOSTIC,
+    ),
     DATA_POINT_LIGHTNING: EntityDescription(
         icon="mdi:map-marker-distance",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_LIGHTNING_NUM: EntityDescription(
         icon="mdi:weather-lightning",
         state_class=StateClass.TOTAL,
@@ -375,26 +382,21 @@
 PLATFORM_MAP = {
     DataPointType.BOOLEAN: Platform.BINARY_SENSOR,
     DataPointType.NON_BOOLEAN: Platform.SENSOR,
 }
 
 STATE_CLASS_OVERRIDES = {
     DATA_POINT_DAILY_RAIN: StateClass.TOTAL,
-    DATA_POINT_DRAIN_PIEZO: StateClass.TOTAL,
-    DATA_POINT_ERAIN_PIEZO: StateClass.TOTAL,
     DATA_POINT_EVENT_RAIN: StateClass.TOTAL,
+    DATA_POINT_GLOB_RAIN_PIEZO: StateClass.TOTAL,
     DATA_POINT_HOURLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_HRAIN_PIEZO: StateClass.TOTAL,
     DATA_POINT_MONTHLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_MRAIN_PIEZO: StateClass.TOTAL,
     DATA_POINT_TOTAL_RAIN: StateClass.TOTAL,
     DATA_POINT_WEEKLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_WRAIN_PIEZO: StateClass.TOTAL,
     DATA_POINT_YEARLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_YRAIN_PIEZO: StateClass.TOTAL,
 }
 
 
 def get_availability_payload(
     data_point: CalculatedDataPoint,
 ) -> str:
     """Get the availability payload for a data point.
@@ -448,42 +450,40 @@
             elif strategy == BatteryStrategy.NUMERIC:
                 data_point_key = DATA_POINT_BATTERY_NUMERIC
             else:
                 data_point_key = DATA_POINT_BATTERY_PERCENTAGE
         else:
             data_point_key = data_point.data_point_key
 
-        if self._config.hass_entity_id_prefix:
-            name = f"{self._config.hass_entity_id_prefix}_{payload_key}"
-        else:
-            name = payload_key
-
         base_topic = (
             f"{self._config.hass_discovery_prefix}/{PLATFORM_MAP[data_point.data_type]}"
             f"/{device.unique_id}/{payload_key}"
         )
 
-        payload = self._discovery_payloads[payload_key] = HassDiscoveryPayload(
-            {
-                "availability_topic": f"{base_topic}/availability",
-                "device": {
-                    "identifiers": [device.unique_id],
-                    "manufacturer": device.manufacturer,
-                    "model": device.model,
-                    "name": device.name,
-                    "sw_version": device.station_type,
-                },
-                "json_attributes_topic": f"{base_topic}/attributes",
-                "name": name,
-                "qos": 1,
-                "retain": self._config.mqtt_retain,
-                "state_topic": f"{base_topic}/state",
-                "unique_id": f"{device.unique_id}_{payload_key}",
+        config = {
+            "availability_topic": f"{base_topic}/availability",
+            "device": {
+                "identifiers": [device.unique_id],
+                "manufacturer": device.manufacturer,
+                "model": device.model,
+                "name": device.name,
+                "sw_version": device.station_type,
             },
-            f"{base_topic}/config",
+            "json_attributes_topic": f"{base_topic}/attributes",
+            "name": payload_key,
+            "qos": 1,
+            "retain": self._config.mqtt_retain,
+            "state_topic": f"{base_topic}/state",
+            "unique_id": f"{device.unique_id}_{payload_key}",
+        }
+        if self._config.hass_entity_id_prefix:
+            config["object_id"] = f"{self._config.hass_entity_id_prefix}_{payload_key}"
+
+        payload = self._discovery_payloads[payload_key] = HassDiscoveryPayload(
+            config, f"{base_topic}/config"
         )
 
         if data_point.attributes:
             payload.payload["json_attributes_topic"] = f"{base_topic}/attributes"
         if data_point.unit:
             payload.payload["unit_of_measurement"] = data_point.unit
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/topic.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/publisher/topic.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/server.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/helpers/server.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/runtime.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import uvicorn
 from asyncio_mqtt import Client, MqttError
 from fastapi import FastAPI
 
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.const import LOGGER
-from ecowitt2mqtt.helpers.publisher.factory import get_publisher
+from ecowitt2mqtt.helpers.publisher.factory import get_publishers
 from ecowitt2mqtt.helpers.server import APIServer, get_api_server
 
 if TYPE_CHECKING:
     from ecowitt2mqtt.core import Ecowitt
 
 DEFAULT_HOST = "0.0.0.0"  # noqa: S104, # nosec: B104
 DEFAULT_MAX_RETRY_INTERVAL = 60
@@ -91,15 +91,15 @@
             config: A Config object.
             queue: An asyncio Queue object.
             payload_event: An asyncio Event object.
 
         Returns:
             An asyncio Task object.
         """
-        LOGGER.debug("Creating MQTT loop: %s", config.mqtt_connection_info)
+        LOGGER.debug("Creating MQTT loop: %s", config.uuid)
 
         async def create_loop() -> None:
             """Create the loop.
 
             Raises:
                 asyncio.CancelledError: Raised when the task is cancelled.
             """
@@ -111,21 +111,25 @@
                             config.mqtt_broker,
                             logger=LOGGER,
                             password=config.mqtt_password,
                             port=config.mqtt_port,
                             tls_context=SSLContext() if config.mqtt_tls else None,
                             username=config.mqtt_username,
                         ) as client:
-                            publisher = get_publisher(config, client)
+                            publishers = get_publishers(config, client)
                             while True:
                                 await payload_event.wait()
                                 while not queue.empty():
                                     payload = await queue.get()
                                     LOGGER.debug("Publishing payload: %s", payload)
-                                    await publisher.async_publish(payload)
+                                    tasks = [
+                                        publisher.async_publish(payload)
+                                        for publisher in publishers
+                                    ]
+                                    await asyncio.gather(*tasks)
 
                                 if config.diagnostics:
                                     LOGGER.info("*** DIAGNOSTICS COLLECTED")
                                     self.stop()
 
                                 payload_event.clear()
                                 retry_attempt = 0
@@ -155,27 +159,21 @@
 
         Args:
             payload: An API request payload.
         """
         config = self.ecowitt.configs.get(payload["PASSKEY"])
 
         # Store the payload in the appropriate queue:
-        queue = self._payload_queues.setdefault(
-            config.mqtt_connection_info, asyncio.Queue()
-        )
+        queue = self._payload_queues.setdefault(config.uuid, asyncio.Queue())
         queue.put_nowait(payload)
 
         # If there isn't an active MQTT loop for this payload, create it first and
         # instruct it to publish the payload once it's connected:
-        if (
-            payload_event := self._payload_events.get(config.mqtt_connection_info)
-        ) is None:
-            payload_event = self._payload_events[
-                config.mqtt_connection_info
-            ] = asyncio.Event()
+        if (payload_event := self._payload_events.get(config.uuid)) is None:
+            payload_event = self._payload_events[config.uuid] = asyncio.Event()
             self._mqtt_loop_tasks.append(
                 self._async_create_mqtt_loop_task(config, queue, payload_event)
             )
 
         payload_event.set()
 
     async def async_start(self) -> None:
```

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/meteo.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/meteo.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/unit_conversion.py` & `ecowitt2mqtt-2023.6.0/ecowitt2mqtt/util/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.5.0/pyproject.toml` & `ecowitt2mqtt-2023.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "ecowitt2mqtt"
-version = "2023.05.0"
+version = "2023.06.0"
 description = "A small web server to send data from Ecowitt devices to an MQTT Broker"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/ecowitt2mqtt"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -59,15 +59,15 @@
 ]
 
 [tool.poetry.dependencies]
 "ruamel.yaml" = "^0.17.21"
 aiohttp = "^3.8.1"
 asyncio-mqtt = ">=0.12.1"
 colorlog = "^6.6.0"
-fastapi = ">=0.89.1,<0.96.0"
+fastapi = ">=0.89.1,<0.98.0"
 meteocalc = "^1.1.0"
 python = "^3.9.0"
 python-multipart = ">=0.0.5,<0.0.7"
 rapidfuzz = ">=2.13,<4.0"
 uvicorn = ">=0.19.0"
 uvloop = "^0.17.0"
 voluptuous = "^0.13.1"
@@ -86,15 +86,16 @@
 pre-commit-hooks = "^4.3.0"
 pylint = "^2.15.5"
 pytest = "^7.2.0"
 pytest-aiohttp = "^1.0.0"
 pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-cov = "^4.0.0"
 pyupgrade = "^3.1.0"
-ruff = ">=0.0.261,<0.0.268"
+requests = ">=2.31.0"
+ruff = ">=0.0.261,<0.0.273"
 safety = "^2.3.1"
 typing-extensions = "^4.4.0"
 vulture = "^2.6"
 yamllint = "^1.28.0"
 
 [tool.poetry.scripts]
 ecowitt2mqtt = "ecowitt2mqtt.__main__:main"
```

### Comparing `ecowitt2mqtt-2023.5.0/PKG-INFO` & `ecowitt2mqtt-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: ecowitt2mqtt
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: A small web server to send data from Ecowitt devices to an MQTT Broker
 Home-page: https://github.com/bachya/ecowitt2mqtt
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: asyncio-mqtt (>=0.12.1)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
-Requires-Dist: fastapi (>=0.89.1,<0.96.0)
+Requires-Dist: fastapi (>=0.89.1,<0.98.0)
 Requires-Dist: meteocalc (>=1.1.0,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.7)
 Requires-Dist: rapidfuzz (>=2.13,<4.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: uvicorn (>=0.19.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: voluptuous (>=0.13.1,<0.14.0)
```

#### html2text {}

```diff
@@ -1,40 +1,38 @@
-Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.5.0 Summary: A small web
+Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.6.0 Summary: A small web
 server to send data from Ecowitt devices to an MQTT Broker Home-page: https://
 github.com/bachya/ecowitt2mqtt License: MIT Author: Aaron Bach Author-email:
 bachya1208@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: asyncio-mqtt (>=0.12.1)
-Requires-Dist: colorlog (>=6.6.0,<7.0.0) Requires-Dist: fastapi
-(>=0.89.1,<0.96.0) Requires-Dist: meteocalc (>=1.1.0,<2.0.0) Requires-Dist:
-python-multipart (>=0.0.5,<0.0.7) Requires-Dist: rapidfuzz (>=2.13,<4.0)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: uvicorn
-(>=0.19.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Requires-Dist: voluptuous
-(>=0.13.1,<0.14.0) Project-URL: Bug Tracker, https://github.com/bachya/
-ecowitt2mqtt/issues Project-URL: Changelog, https://github.com/bachya/
-ecowitt2mqtt/releases Project-URL: Repository, https://github.com/bachya/
-ecowitt2mqtt Description-Content-Type: text/markdown ![ecowitt2mqtt][logo] [!
-[CI][ci-badge]][ci] [![PyPI][pypi-badge]][pypi] [![Docker Hub][docker-hub-
-badge]][docker-hub] [![Version][version-badge]][version] [![License][license-
-badge]][license] [![Code Coverage][codecov-badge]][codecov] [![Maintainability]
-[maintainability-badge]][maintainability] [Buy_Me_A_Coffee] `ecowitt2mqtt` is a
-small CLI/web server that can receive data from Fine Offset weather stations
-(and their numerous white-labeled counterparts, like Ecowitt and Ambient
-Weather), adjust that data in numerous ways, and send it on to one or more MQTT
-brokers. - [Installation](#installation) - [Python Versions](#python-versions)
-- [Disclaimer](#disclaimer) - [Supported Brands](#supported-brands) - [Quick
-Start](#quick-start) - [Configuration](#configuration) - [Command Line Options]
-(#command-line-options) - [Environment Variables](#environment-variables) -
+Python :: Implementation :: CPython Classifier: Programming Language :: Python
+:: Implementation :: PyPy Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
+Dist: asyncio-mqtt (>=0.12.1) Requires-Dist: colorlog (>=6.6.0,<7.0.0)
+Requires-Dist: fastapi (>=0.89.1,<0.98.0) Requires-Dist: meteocalc
+(>=1.1.0,<2.0.0) Requires-Dist: python-multipart (>=0.0.5,<0.0.7) Requires-
+Dist: rapidfuzz (>=2.13,<4.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: uvicorn (>=0.19.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0)
+Requires-Dist: voluptuous (>=0.13.1,<0.14.0) Project-URL: Bug Tracker, https://
+github.com/bachya/ecowitt2mqtt/issues Project-URL: Changelog, https://
+github.com/bachya/ecowitt2mqtt/releases Project-URL: Repository, https://
+github.com/bachya/ecowitt2mqtt Description-Content-Type: text/markdown !
+[ecowitt2mqtt][logo] [![CI][ci-badge]][ci] [![PyPI][pypi-badge]][pypi] [!
+[Docker Hub][docker-hub-badge]][docker-hub] [![Version][version-badge]]
+[version] [![License][license-badge]][license] [![Code Coverage][codecov-
+badge]][codecov] [![Maintainability][maintainability-badge]][maintainability]
+[Buy_Me_A_Coffee] `ecowitt2mqtt` is a small CLI/web server that can receive
+data from Fine Offset weather stations (and their numerous white-labeled
+counterparts, like Ecowitt and Ambient Weather), adjust that data in numerous
+ways, and send it on to one or more MQTT brokers. - [Installation]
+(#installation) - [Python Versions](#python-versions) - [Disclaimer]
+(#disclaimer) - [Supported Brands](#supported-brands) - [Quick Start](#quick-
+start) - [Configuration](#configuration) - [Command Line Options](#command-
+line-options) - [Environment Variables](#environment-variables) -
 [Configuration File](#configuration-file) - [Merging Configuration Options]
 (#merging-configuration-options) - [Input Data Formats](#input-data-formats) -
 [Advanced Usage](#advanced-usage) - [Calculated Sensors](#calculated-sensors) -
 [Battery Configurations](#battery-configurations) - [Unit Systems](#unit-
 systems) - [Raw Data](#raw-data) - [Home Assistant](#home-assistant) - [Running
 in the Background](#running-in-the-background) - [Docker](#docker) -
 [Diagnostics](#diagnostics) - [Contributing](#contributing) # Installation
```

