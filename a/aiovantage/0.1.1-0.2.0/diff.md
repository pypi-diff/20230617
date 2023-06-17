# Comparing `tmp/aiovantage-0.1.1.tar.gz` & `tmp/aiovantage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiovantage-0.1.1.tar", last modified: Fri Jun 16 06:42:14 2023, max compression
+gzip compressed data, was "aiovantage-0.2.0.tar", last modified: Sat Jun 17 06:34:47 2023, max compression
```

## Comparing `aiovantage-0.1.1.tar` & `aiovantage-0.2.0.tar`

### file list

```diff
@@ -1,158 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.843158 aiovantage-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.811159 aiovantage-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 06:42:00.000000 aiovantage-0.1.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 06:42:00.000000 aiovantage-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 06:42:00.000000 aiovantage-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-16 06:42:14.843158 aiovantage-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-16 06:42:00.000000 aiovantage-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/examples/areas/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/areas/dump_areas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/examples/blind_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/blind_groups/dump_blind_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/blinds/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/blinds/dump_blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/blinds/monitor_blinds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/buttons/dump_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/buttons/monitor_buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/command_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/command_client/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/command_client/status_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/config_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/config_client/dump_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/config_client/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/dry_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/dump_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/gmem/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/gmem/dump_gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/gmem/monitor_gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/gmem/set_gmem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/load_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/load_groups/dump_load_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/loads/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/control_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/dump_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/monitor_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/poll_on_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/toggle_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/monitor_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/omni_sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/omni_sensors/monitor_omni_sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/examples/rgb_loads/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/rgb_loads/monitor_rgb_loads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/examples/stations/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/stations/dump_stations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/examples/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/tasks/dump_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/tasks/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 06:42:00.000000 aiovantage-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:42:14.843158 aiovantage-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.815158 aiovantage-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/src/aiovantage/
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/src/aiovantage/command_client/
--rw-r--r--   0 runner    (1001) docker     (123)    29576 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/object_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/open_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.835158 aiovantage-0.1.1/src/aiovantage/config_client/methods/login/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.839158 aiovantage-0.1.1/src/aiovantage/config_client/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/urtsi_2_group_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/urtsi_2_shade_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/xml_dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.843158 aiovantage-0.1.1/src/aiovantage/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/areas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/gmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/loads.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/masters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/src/aiovantage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.867621 aiovantage-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.843620 aiovantage-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-17 06:34:36.000000 aiovantage-0.2.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-17 06:34:36.000000 aiovantage-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-17 06:34:36.000000 aiovantage-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 06:34:47.867621 aiovantage-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-17 06:34:36.000000 aiovantage-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/areas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/areas/dump_areas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/blind_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/blind_groups/dump_blind_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/blinds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/blinds/monitor_blinds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/buttons/monitor_buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/examples/command_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/command_client/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/command_client/status_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/config_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/config_client/dump_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/config_client/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/dry_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/dump_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/gmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/gmem/set_gmem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/load_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/load_groups/dump_load_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/control_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/dump_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/monitor_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/loads/toggle_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/monitor_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/omni_sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/omni_sensors/monitor_omni_sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/rgb_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/rgb_loads/monitor_rgb_loads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/stations/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/stations/dump_stations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/examples/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-17 06:34:36.000000 aiovantage-0.2.0/examples/tasks/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-17 06:34:36.000000 aiovantage-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 06:34:47.867621 aiovantage-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.847620 aiovantage-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/src/aiovantage/
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/command_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30612 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/command_client/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/config_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.855621 aiovantage-0.2.0/src/aiovantage/config_client/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.859621 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/object_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/open_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.859621 aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.859621 aiovantage-0.2.0/src/aiovantage/config_client/methods/login/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/methods/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.863621 aiovantage-0.2.0/src/aiovantage/config_client/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/urtsi_2_group_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/objects/urtsi_2_shade_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/config_client/xml_dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.867621 aiovantage-0.2.0/src/aiovantage/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-17 06:34:36.000000 aiovantage-0.2.0/src/aiovantage/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:34:47.851620 aiovantage-0.2.0/src/aiovantage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 06:34:47.000000 aiovantage-0.2.0/src/aiovantage.egg-info/top_level.txt
```

### Comparing `aiovantage-0.1.1/.github/workflows/publish-to-test-pypi.yml` & `aiovantage-0.2.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/LICENSE` & `aiovantage-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/PKG-INFO` & `aiovantage-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python module to talk to Vantage InFusion controllers.
 Author-email: James Smith <james@loopj.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiovantage-0.1.1/README.md` & `aiovantage-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/areas/dump_areas.py` & `aiovantage-0.2.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.2.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/blinds/dump_blinds.py` & `aiovantage-0.2.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/blinds/monitor_blinds.py` & `aiovantage-0.2.0/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/buttons/dump_buttons.py` & `aiovantage-0.2.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/buttons/monitor_buttons.py` & `aiovantage-0.2.0/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/command_client/event_log.py` & `aiovantage-0.2.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/command_client/status_load.py` & `aiovantage-0.2.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/config_client/dump_objects.py` & `aiovantage-0.2.0/examples/config_client/dump_objects.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import asyncio
 import logging
 
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.helpers import get_objects_by_type
-from aiovantage.config_client.objects import Area, Load, StationObject
+from aiovantage.config_client.helpers import get_objects
 
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
@@ -16,34 +15,30 @@
 args = parser.parse_args()
 
 
 async def main() -> None:
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    async with ConfigClient(
-        args.host, args.username, args.password
-    ) as client:
-        # Dump all Areas using the get_objects_by_type helper
+    async with ConfigClient(args.host, args.username, args.password) as client:
+        # Dump all Areas using the get_objects helper
         print("# Vantage Areas")
-        async for area in get_objects_by_type(client, ["Area"], Area):
+        async for area in get_objects(client, type="Area"):
             print(area)
         print()
 
-        # Dump all Loads using the get_objects_by_type helper
+        # Dump all Loads using the get_objects helper
         print("# Vantage Loads")
-        async for load in get_objects_by_type(client, ["Load"], Load):
+        async for load in get_objects(client, type="Load"):
             print(load)
         print()
 
-        # Dump some StationObjects using the get_objects_by_type helper
+        # Dump some StationObjects using the get_objects helper
         print("# Vantage Stations")
-        async for station in get_objects_by_type(
-            client, ["Keypad", "EqCtrl"], StationObject
-        ):
+        async for station in get_objects(client, type=("Keypad", "EqCtrl")):
             print(station)
         print()
 
 
 try:
     asyncio.run(main())
 except KeyboardInterrupt:
```

### Comparing `aiovantage-0.1.1/examples/config_client/get_version.py` & `aiovantage-0.2.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.2.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.2.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/dump_system.py` & `aiovantage-0.2.0/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/gmem/dump_gmem.py` & `aiovantage-0.2.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/gmem/monitor_gmem.py` & `aiovantage-0.2.0/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/gmem/set_gmem.py` & `aiovantage-0.2.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/load_groups/dump_load_groups.py` & `aiovantage-0.2.0/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/loads/control_load.py` & `aiovantage-0.2.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/loads/dump_loads.py` & `aiovantage-0.2.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/loads/monitor_loads.py` & `aiovantage-0.2.0/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/loads/poll_on_loads.py` & `aiovantage-0.2.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/loads/toggle_load.py` & `aiovantage-0.2.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/monitor_all.py` & `aiovantage-0.2.0/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.2.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.2.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.2.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.2.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/stations/dump_stations.py` & `aiovantage-0.2.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/tasks/dump_tasks.py` & `aiovantage-0.2.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/examples/tasks/run_task.py` & `aiovantage-0.2.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/pyproject.toml` & `aiovantage-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "xsdata==23.5",
+    "typing_extensions>=4.4.0,<5; python_version < '3.12'",
 ]
 dynamic = ["version"]
 
 [tool.setuptools_scm]
 
 [tool.isort]
 profile = "black"
```

### Comparing `aiovantage-0.1.1/src/aiovantage/__init__.py` & `aiovantage-0.2.0/src/aiovantage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __all__ = ["Vantage", "VantageEvent"]
 
 import asyncio
 from types import TracebackType
 from typing import Callable, Optional, Type
 
+from typing_extensions import Self
+
 from aiovantage.command_client import CommandClient
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.objects import SystemObject
 from aiovantage.controllers.areas import AreasController
 from aiovantage.controllers.base import EventCallback
 from aiovantage.controllers.blinds import BlindsController
 from aiovantage.controllers.blind_groups import BlindGroupsController
@@ -60,25 +62,28 @@
         self._load_groups = LoadGroupsController(self)
         self._masters = MastersController(self)
         self._rgb_loads = RGBLoadsController(self)
         self._omni_sensors = OmniSensorsController(self)
         self._stations = StationsController(self)
         self._tasks = TasksController(self)
 
-    async def __aenter__(self) -> "Vantage":
+    async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
+        exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         await self.close()
 
+        if exc_val:
+            raise exc_val
+
     @property
     def config_client(self) -> ConfigClient:
         """Return the config client."""
         return self._config_client
 
     @property
     def command_client(self) -> CommandClient:
```

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/__init__.py` & `aiovantage-0.2.0/src/aiovantage/command_client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     "ClientTimeoutError",
     "CommandError",
     "LoginFailedError",
     "LoginRequiredError",
 ]
 
 import asyncio
-from decimal import Decimal
 import logging
 from collections import defaultdict
 from contextlib import suppress
 from dataclasses import dataclass
+from decimal import Decimal
 from inspect import iscoroutinefunction
 from ssl import SSLContext
 from types import TracebackType
 from typing import (
     AsyncIterator,
     Awaitable,
     Callable,
@@ -46,26 +46,29 @@
     Optional,
     Set,
     Tuple,
     Type,
     Union,
 )
 
+from typing_extensions import Self
+
 from .errors import (
     ClientConnectionError,
     ClientError,
     ClientTimeoutError,
     CommandError,
     LoginFailedError,
     LoginRequiredError,
 )
 from .events import Event, EventType
-from .helpers import tokenize_response, encode_params
+from .helpers import encode_params, tokenize_response
 from .ssl import create_ssl_context
 
+KEEPALIVE_INTERVAL = 60
 
 # Type aliases for callbacks for event subscriptions
 EventCallback = Union[Callable[[Event], None], Callable[[Event], Awaitable[None]]]
 EventFilter = Callable[[Event], bool]
 EventSubscription = Tuple[EventCallback, Optional[EventFilter]]
 
 
@@ -152,26 +155,29 @@
         # Set up the port
         self._port: int
         if port is None:
             self._port = 3010 if ssl else 3001
         else:
             self._port = port
 
-    async def __aenter__(self) -> "CommandConnection":
+    async def __aenter__(self) -> Self:
         await self.open()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
+        exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         self.close()
 
+        if exc_val:
+            raise exc_val
+
     async def open(self) -> None:
         """Open a connection to the Vantage Host Command service."""
 
         # If we're already connected, do nothing
         if self._writer is not None and not self._writer.is_closing():
             return
 
@@ -244,64 +250,61 @@
         else:
             request = command
 
         # Send the request and wait for the response as a single transaction
         async with self._command_lock:
             # Send the request
             try:
-                self._logger.debug(f"Sending command: {request}")
+                self._logger.debug("Sending command: %s", request)
                 self._writer.write(f"{request}\n".encode())
                 await self._writer.drain()
             except OSError as exc:
                 raise ClientConnectionError("Connection error") from exc
 
             # Wait for the response
             try:
                 response = await asyncio.wait_for(
                     self._response_queue.get(), timeout=self._read_timeout
                 )
-                self._logger.debug(f"Received response: {response}")
+                self._logger.debug("Received response: %s", response)
             except asyncio.TimeoutError as exc:
                 raise ClientTimeoutError("Timeout waiting for response") from exc
 
-        # Handle exception fetched from the queue
-        if isinstance(response, CommandError):
-            # R:ERROR responses
-            raise response
-        elif isinstance(response, (OSError, asyncio.IncompleteReadError)):
-            # Connection errors, or EOF when reading response
+        # Re-raise connection errors, EOF, etc. as a connection error
+        if isinstance(response, (OSError, asyncio.IncompleteReadError)):
             raise ClientConnectionError("Connection error") from response
-        elif isinstance(response, Exception):
-            # Other unexpected errors
-            raise
+
+        # Re-raise all other exceptions, including "R:ERROR" responses
+        if isinstance(response, Exception):
+            raise response
 
         return response
 
     async def events(self) -> AsyncIterator[str]:
         """
         An async iterator that yields events from the Host Command service.
 
         Yields:
             "S:" (Status) or "EL:" (Event Log) strings from the Host Command service.
         """
 
-        queue = asyncio.Queue[Union[str, Exception]](1024)
+        queue: asyncio.Queue[Union[str, Exception]] = asyncio.Queue(1024)
         try:
             self._event_queues.add(queue)
 
             while True:
                 event = await queue.get()
 
-                # Handle exception fetched from the queue
+                # Re-raise connection errors, EOF, etc. as a connection error
                 if isinstance(event, (OSError, asyncio.IncompleteReadError)):
-                    # Connection errors, or EOF when reading response
                     raise ClientConnectionError("Connection error") from event
-                elif isinstance(event, Exception):
-                    # Other unexpected errors
-                    raise
+
+                # Re-raise all other exceptions
+                if isinstance(event, Exception):
+                    raise event
 
                 yield event
         finally:
             self._event_queues.remove(queue)
 
     async def _message_handler(self) -> None:
         # Task to handle potentially interleaved incoming messages from the Host Command
@@ -320,54 +323,58 @@
                     self._response_buffer.append(message)
                     self._put_response(CommandResponse(self._response_buffer))
                     self._response_buffer = []
                 elif message.startswith("S:") or message.startswith("EL:"):
                     self._put_event(message)
                 else:
                     self._response_buffer.append(message)
-            except Exception as e:
-                self._put_response(e, warn=False)
-                self._put_event(e)
+            except Exception as exc:
+                self._put_response(exc, warn=False)
+                self._put_event(exc)
                 break
 
         # Explicitly close the connection
         if self._writer is not None and not self._writer.is_closing():
             self._writer.close()
             self._writer = None
 
     def _put_event(self, event: Union[str, Exception]) -> None:
         # Send an event to all event queues.
 
         for queue in self._event_queues:
             if queue.full():
                 dropped_event = queue.get_nowait()
                 self._logger.warning(
-                    f"Event queue full trying to put '{event}', dropping oldest event"
-                    f"'{dropped_event}' to make room."
+                    "Event queue full trying to put '%s', "
+                    "dropping oldest event '%s' to make room.",
+                    event,
+                    dropped_event,
                 )
 
             queue.put_nowait(event)
 
     def _put_response(
         self, response: Union[CommandResponse, Exception], warn: bool = True
     ) -> None:
         # Send a response to the response queue, discard if no command is waiting.
 
         if self._command_lock.locked():
             if not self._response_queue.empty():
                 old_response = self._response_queue.get_nowait()
                 self._logger.error(
-                    f"Response queue not empty when trying to put '{response}', "
-                    f"dropping previous response '{old_response}'."
+                    "Response queue not empty when trying to put '%s', "
+                    "dropping previous response '%s'.",
+                    response,
+                    old_response,
                 )
 
             self._response_queue.put_nowait(response)
         elif warn:
             self._logger.error(
-                f"Discarding response message, no command waiting: {response}"
+                "Discarding response message, no command waiting: %s", response
             )
 
 
 class CommandClient:
     """
     High-level client to communicate with the Vantage InFusion "Host Command" service.
 
@@ -413,63 +420,72 @@
         self._port = port
         self._conn_timeout = conn_timeout
         self._read_timeout = read_timeout
 
         self._connection: Optional[CommandConnection] = None
         self._event_handler_task: Optional[asyncio.Task[None]] = None
         self._event_handler_ready: asyncio.Event = asyncio.Event()
+        self._keepalive_task: Optional[asyncio.Task[None]] = None
         self._subscriptions: List[EventSubscription] = []
         self._subscribed_statuses: Dict[str, int] = defaultdict(int)
         self._subscribed_objects: Dict[int, int] = defaultdict(int)
         self._subscribed_event_logs: Dict[str, int] = defaultdict(int)
         self._logger = logging.getLogger(__name__)
         self._lock = asyncio.Lock()
 
-    async def __aenter__(self) -> "CommandClient":
+    async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
+        exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         await self.close()
 
+        if exc_val:
+            raise exc_val
+
     async def connection(self, retry: bool = False) -> CommandConnection:
         """
         Get a connection to the Host Command service, creating one if necessary.
 
         Args:
             retry: Whether to retry if the connection attempt fails.
         """
 
         try:
             # Note: Getting a connection can potentially block for a long time even if
             # retry is False, if someone else is already trying to get a connection.
             await asyncio.wait_for(
                 self._lock.acquire(), timeout=(None if retry else self._conn_timeout)
             )
-        except asyncio.TimeoutError:
-            raise ClientTimeoutError("Timeout waiting for connection")
+        except asyncio.TimeoutError as exc:
+            raise ClientTimeoutError("Timeout waiting for connection") from exc
 
         try:
             if self._connection is None or self._connection.closed:
                 self._connection = await self._create_connection(retry=retry)
 
             return self._connection
         finally:
             self._lock.release()
 
     async def close(self) -> None:
         """
-        Close the connections to the Host Command service and stop the event handler.
+        Close the connections to the Host Command service and cancel any running tasks.
         """
 
-        # Stop the event handler
+        # Cancel the keepalive task
+        if self._keepalive_task is not None:
+            self._keepalive_task.cancel()
+            self._keepalive_task = None
+
+        # Cancel the event handler task
         if self._event_handler_task is not None:
             self._event_handler_task.cancel()
             self._event_handler_task = None
 
         # Close the connections
         if self._connection is not None:
             self._connection.close()
@@ -726,22 +742,23 @@
                 if not retry:
                     raise
 
             # Attempt to reconnect, with backoff
             reconnect_wait = min(2 * connect_attempts, 600)
 
             self._logger.debug(
-                f"Connection to {self._host} failed"
-                f" - retrying in {reconnect_wait} seconds"
+                "Connection to controller failed - retrying in %d seconds",
+                reconnect_wait,
             )
 
             if connect_attempts % 10 == 0:
                 self._logger.warning(
-                    f"{connect_attempts} attempts to (re)connect to {self._host} failed"
-                    f" - this may indicate a problem with the connection"
+                    "%d attempts to (re)connect to controller failed"
+                    " - This might be an indication of connection issues.",
+                    connect_attempts,
                 )
 
             await asyncio.sleep(reconnect_wait)
 
     async def _resubscribe(self, conn: CommandConnection) -> None:
         # Re-subscribe to events after a reconnection
 
@@ -775,30 +792,32 @@
                     self._emit({"tag": EventType.RECONNECTED})
                 else:
                     self._event_handler_ready.set()
                     self._emit({"tag": EventType.CONNECTED})
 
                 self._logger.info("Event handler connected and listening for events")
 
+                # Start the keepalive task
+                self._keepalive_task = asyncio.create_task(self._keepalive())
+
                 # Start processing events
                 async for event in conn.events():
-                    self._logger.debug(f"Received event: {event}")
+                    self._logger.debug("Received event: %s", event)
 
                     if event.startswith("S:"):
                         # Parse a status message
                         status_type, id_str, *args = tokenize_response(event)
                         status_type = status_type[2:]
-                        id = int(id_str)
 
                         # Notify subscribers
                         self._emit(
                             {
                                 "tag": EventType.STATUS,
                                 "status_type": status_type,
-                                "id": id,
+                                "id": int(id_str),
                                 "args": args,
                             },
                         )
                     elif event.startswith("EL:"):
                         # Parse an event log message
                         message = event[4:]
 
@@ -806,18 +825,37 @@
                         self._emit(
                             {
                                 "tag": EventType.EVENT_LOG,
                                 "log": message,
                             },
                         )
                     else:
-                        self._logger.warning(f"Received unexpected event: {event}")
+                        self._logger.warning("Received unexpected event: %s", event)
 
             except ClientConnectionError:
-                # If we get here, the connection was lost
-                self._logger.debug("Event handler lost connection", exc_info=True)
-                self._emit({"tag": EventType.DISCONNECTED})
+                pass
 
             except Exception:
                 # Unexpected error, log for debugging
                 self._logger.exception("Unexpected error in event handler")
                 raise
+
+            # If we get here, the connection was lost
+            self._logger.debug("Event handler lost connection")
+            self._emit({"tag": EventType.DISCONNECTED})
+
+            # Cancel the keepalive task
+            if self._keepalive_task is not None:
+                self._keepalive_task.cancel()
+                self._keepalive_task = None
+
+    async def _keepalive(self) -> None:
+        # Send an "ECHO" command periodically to keep the connection alive,
+        # and detect dropped connections.
+
+        while True:
+            await asyncio.sleep(KEEPALIVE_INTERVAL)
+
+            try:
+                await self.command("ECHO")
+            except ClientError as err:
+                self._logger.debug("Error while sending keepalive: %s", str(err))
```

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/errors.py` & `aiovantage-0.2.0/src/aiovantage/command_client/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/events.py` & `aiovantage-0.2.0/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/helpers.py` & `aiovantage-0.2.0/src/aiovantage/command_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
         """
 
         # ELLOG STATUS ON
         # -> EL: <id> Sensor.GetLevel <level>
 
         # STATUS ADD <id>
         # -> S:STATUS <id> Sensor.GetLevel <level>
-        return int(args[0])
+        return int(args[0])
```

### Comparing `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.2.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/__init__.py` & `aiovantage-0.2.0/src/aiovantage/config_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 import asyncio
 import logging
 import ssl
 import xml.etree.ElementTree as ET
 from types import TracebackType
 from typing import Any, Optional, Tuple, Type, Union
 
+from typing_extensions import Self
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import XmlEventHandler
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
+from .errors import ClientConnectionError, ClientTimeoutError
 from .methods import CallType, Method, ReturnType
 from .methods.login import Login
 
 # Type alias for connections
 Connection = Tuple[asyncio.StreamReader, asyncio.StreamWriter]
 
 
@@ -104,25 +106,28 @@
             handler=XmlEventHandler,
         )
 
         self._serializer = XmlSerializer(
             config=SerializerConfig(xml_declaration=False),
         )
 
-    async def __aenter__(self) -> "ConfigClient":
+    async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         self.close()
 
+        if exc_val:
+            raise exc_val
+
     def close(self) -> None:
         """
         Close any open connections to the ACI service.
         """
 
         # Check if connection is already closed
         if self._connection is None or self._connection[1].is_closing():
@@ -130,39 +135,46 @@
 
         # Close the connection
         _, writer = self._connection
         writer.close()
 
         self._logger.debug("Connection closed")
 
-    async def raw_request(self, request_payload: str, end_token: str) -> str:
+    async def raw_request(self, interface: str, payload: str) -> str:
         """
         Send a plaintext request to the ACI service.
 
         Args:
-            request_payload: The request payload string to send
-            end_token: The token to look for to indicate the end of the response
+            interface: The interface to send the request to
+            payload: The request payload string to send
 
         Returns:
             The response payload string
         """
 
         async with self._lock:
             # Get a connection
             reader, writer = await self._get_connection()
 
-            # Send the request
-            writer.write(request_payload.encode())
-            await writer.drain()
-
-            # Fetch the response
-            end_bytes = end_token.encode()
-            data = await asyncio.wait_for(
-                reader.readuntil(end_bytes), timeout=self._read_timeout
-            )
+            try:
+                # Send the request
+                request = f"<{interface}>{payload}</{interface}>"
+                writer.write(request.encode())
+                await writer.drain()
+
+                # Fetch the response
+                end_bytes = f"</{interface}>\n".encode()
+                data = await asyncio.wait_for(
+                    reader.readuntil(end_bytes), timeout=self._read_timeout
+                )
+
+            except asyncio.TimeoutError as err:
+                raise ClientTimeoutError from err
+            except (OSError, asyncio.IncompleteReadError) as err:
+                raise ClientConnectionError from err
 
             return data.decode()
 
     async def request(
         self, method: Type[Method[CallType, ReturnType]], params: Any = None
     ) -> ReturnType:
         """
@@ -175,60 +187,63 @@
         Returns:
             The parsed response object
         """
 
         request = self._marshall_request(method, params)
         self._logger.debug(request)
 
-        response = await self.raw_request(request, f"</{method.interface}>\n")
+        response = await self.raw_request(method.interface, request)
         self._logger.debug(response)
 
         return self._unmarshall_response(method, response)
 
     async def _get_connection(self) -> Connection:
         """
         Get a connection to the ACI service, authenticating if necessary.
         """
 
         # If we already have a connection, return it
         if self._connection is not None and not self._connection[1].is_closing():
             return self._connection
 
-        # Otherwise, open a new connection
-        connection = await asyncio.wait_for(
-            asyncio.open_connection(
-                self._host,
-                self._port,
-                ssl=self._ssl_context,
-            ),
-            timeout=self._conn_timeout,
-        )
-        self._connection = connection
-        self._logger.info("Connected")
+        try:
+            # Otherwise, open a new connection
+            connection = await asyncio.wait_for(
+                asyncio.open_connection(
+                    self._host,
+                    self._port,
+                    ssl=self._ssl_context,
+                    limit=2**20,
+                ),
+                timeout=self._conn_timeout,
+            )
+            self._connection = connection
+            self._logger.info("Connected")
+
+            # Login if we have a username and password
+            await self._login()
 
-        # Login if we have a username and password
-        await self._login()
+        except asyncio.TimeoutError as err:
+            raise ClientTimeoutError from err
+        except OSError as err:
+            raise ClientConnectionError from err
 
         return connection
 
     def _marshall_request(
         self, method_cls: Type[Method[CallType, ReturnType]], params: Any
     ) -> str:
         # Serialize the request to XML using xsdata
 
         # Build the method object
         method = method_cls()
         method.call = params
 
         # Render the method object to XML with xsdata
-        return (
-            f"<{method.interface}>"
-            f"{self._serializer.render(method)}"
-            f"</{method.interface}>"
-        )
+        return self._serializer.render(method)
 
     def _unmarshall_response(
         self, method_cls: Type[Method[CallType, ReturnType]], response_str: str
     ) -> ReturnType:
         # Deserialize the response from XML using xsdata
 
         # Parse the XML doc
```

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/helpers.py` & `aiovantage-0.2.0/src/aiovantage/config_client/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-from typing import Any, AsyncIterator, Sequence
+from typing import Any, AsyncIterator, Optional, Sequence
 
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.methods.configuration import (
     CloseFilter,
     GetFilterResults,
     GetObject,
     OpenFilter,
 )
 
 
-async def get_objects_by_type(
-    client: ConfigClient, types: Sequence[str]
+async def get_objects(
+    client: ConfigClient,
+    *,
+    type: Optional[Sequence[str]] = None,
+    xpath: Optional[str] = None,
 ) -> AsyncIterator[Any]:
     """
     Helper function to get all vantage system objects of the specified types
 
     Args:
         client: The ACI client instance
-        types: A list of strings of the Vantage object types to fetch
+        object_types: An optional string, or list of strings of object types to fetch
+        xpath: An optional xpath to filter the results by, eg. "/Load", "/*[@VID='12']"
 
     Yields:
         The objects of the specified types
     """
 
-    try:
-        # Open the filter
-        handle = await client.request(
-            OpenFilter,
-            OpenFilter.Params(objects=OpenFilter.Filter(object_type=list(types))),
-        )
+    # Support both a single object type and a list of status types
+    if isinstance(type, str):
+        type_filter = OpenFilter.Filter(object_type=[type])
+    elif type is None:
+        type_filter = None
+    else:
+        type_filter = OpenFilter.Filter(object_type=list(type))
+
+    # Open the filter
+    handle = await client.request(
+        OpenFilter, OpenFilter.Params(objects=type_filter, xpath=xpath)
+    )
 
+    try:
         # Get the results
         while True:
             response = await client.request(
                 GetFilterResults, GetFilterResults.Params(h_filter=handle)
             )
 
             if not response.objects:
```

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/object_choice.py` & `aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/object_choice.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
                 {
                     "name": xml_tag_from_class(cls),
                     "type": cls,
                 }
                 for cls in ALL_OBJECT_TYPES
             ],
         },
-    )
+    )
```

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.2.0/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.2.0/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from typing import ClassVar, Optional
 
 from aiovantage.config_client.xml_dataclass import xml_element
 
+
 @dataclass
 class GetVersion:
     interface: ClassVar[str] = "IIntrospection"
     call: Optional[object] = None
     return_value: Optional["GetVersion.Return"] = xml_element("return", default=None)
 
     @dataclass
```

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/blind.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from decimal import Decimal
 from typing import Optional
 
 from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element
 
 from .location_object import LocationObject
 
+
 @dataclass
 class Blind(LocationObject):
     parent_id: Optional[int] = xml_element("Parent", default=None)
     orientation: Optional[str] = xml_attribute("ShadeOrientation", default=None)
     type: Optional[str] = xml_attribute("ShadeType", default=None)
 
     def __post_init__(self) -> None:
```

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/gmem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from typing import Union
 
 from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element, xml_text
 
 from .system_object import SystemObject
 
+
 @dataclass
 class GMem(SystemObject):
     @dataclass
     class Tag:
         type: str = xml_text()
         object: bool = xml_attribute("object", default=False)
```

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.2.0/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.2.0/src/aiovantage/config_client/xml_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 def xml_element(name: str, **kwargs: Any) -> Any:
     metadata = {}
     metadata.update(kwargs.pop("metadata", {}))
     metadata.update({"name": name, "type": "Element"})
 
     return field(metadata=metadata, **kwargs)
 
+
 def xml_text(**kwargs: Any) -> Any:
     metadata = {}
     metadata.update(kwargs.pop("metadata", {}))
     metadata.update({"type": "Text"})
 
     return field(metadata=metadata, **kwargs)
 
+
 def xml_tag_from_class(cls: Type[Any]) -> str:
     """Get the XML tag name for a class."""
 
     meta = cls.Meta if "Meta" in cls.__dict__ else None
     name = getattr(meta, "name", cls.__qualname__)
 
     return name
```

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/base.py` & `aiovantage-0.2.0/src/aiovantage/controllers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Union,
     cast,
 )
 
 from aiovantage.command_client import CommandClient, Event, EventType
 from aiovantage.command_client.helpers import tokenize_response
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.helpers import get_objects_by_type
+from aiovantage.config_client.helpers import get_objects
 from aiovantage.config_client.objects import SystemObject
 from aiovantage.events import VantageEvent
 from aiovantage.query import QuerySet
 
 if TYPE_CHECKING:
     from aiovantage import Vantage
 
@@ -83,15 +83,15 @@
         Fetch all objects managed by this controller.
         """
 
         # TODO: Allow re-fetching objects
         # - fire OBJECT_ADDED events for new objects
         # - fire OBJECT_REMOVED events for removed objects
 
-        async for obj in get_objects_by_type(self.config_client, self.vantage_types):
+        async for obj in get_objects(self.config_client, type=self.vantage_types):
             self._items[obj.id] = cast(T, obj)
             self.emit(VantageEvent.OBJECT_ADDED, cast(T, obj))
 
         self._logger.info(f"{self.__class__.__name__} fetched objects")
 
     def subscribe(
         self,
```

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.2.0/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/blinds.py` & `aiovantage-0.2.0/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/buttons.py` & `aiovantage-0.2.0/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.2.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/gmem.py` & `aiovantage-0.2.0/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.2.0/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/loads.py` & `aiovantage-0.2.0/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.2.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.2.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/controllers/tasks.py` & `aiovantage-0.2.0/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage/query.py` & `aiovantage-0.2.0/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.1/src/aiovantage.egg-info/PKG-INFO` & `aiovantage-0.2.0/src/aiovantage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python module to talk to Vantage InFusion controllers.
 Author-email: James Smith <james@loopj.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiovantage-0.1.1/src/aiovantage.egg-info/SOURCES.txt` & `aiovantage-0.2.0/src/aiovantage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/aiovantage/events.py
 src/aiovantage/query.py
 src/aiovantage.egg-info/PKG-INFO
 src/aiovantage.egg-info/SOURCES.txt
 src/aiovantage.egg-info/dependency_links.txt
 src/aiovantage.egg-info/requires.txt
 src/aiovantage.egg-info/top_level.txt
+src/aiovantage/command_client/README.md
 src/aiovantage/command_client/__init__.py
 src/aiovantage/command_client/errors.py
 src/aiovantage/command_client/events.py
 src/aiovantage/command_client/helpers.py
 src/aiovantage/command_client/ssl.py
 src/aiovantage/command_client/interfaces/__init__.py
 src/aiovantage/command_client/interfaces/base.py
@@ -54,15 +55,17 @@
 src/aiovantage/command_client/interfaces/gmem.py
 src/aiovantage/command_client/interfaces/introspection.py
 src/aiovantage/command_client/interfaces/load.py
 src/aiovantage/command_client/interfaces/object.py
 src/aiovantage/command_client/interfaces/rgb_load.py
 src/aiovantage/command_client/interfaces/sensor.py
 src/aiovantage/command_client/interfaces/task.py
+src/aiovantage/config_client/README.md
 src/aiovantage/config_client/__init__.py
+src/aiovantage/config_client/errors.py
 src/aiovantage/config_client/helpers.py
 src/aiovantage/config_client/xml_dataclass.py
 src/aiovantage/config_client/methods/__init__.py
 src/aiovantage/config_client/methods/configuration/__init__.py
 src/aiovantage/config_client/methods/configuration/close_filter.py
 src/aiovantage/config_client/methods/configuration/get_filter_results.py
 src/aiovantage/config_client/methods/configuration/get_object.py
```

