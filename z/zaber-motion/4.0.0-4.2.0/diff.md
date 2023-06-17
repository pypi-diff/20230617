# Comparing `tmp/zaber_motion-4.0.0.tar.gz` & `tmp/zaber_motion-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-4.0.0.tar", last modified: Mon Jun  5 20:45:30 2023, max compression
+gzip compressed data, was "zaber_motion-4.2.0.tar", last modified: Sat Jun 17 02:49:41 2023, max compression
```

## Comparing `zaber_motion-4.0.0.tar` & `zaber_motion-4.2.0.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.898172 zaber_motion-4.0.0/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-05 20:45:30.898234 zaber_motion-4.0.0/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-06-05 20:45:30.898479 zaber_motion-4.0.0/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.877399 zaber_motion-4.0.0/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.879248 zaber_motion-4.0.0/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.885537 zaber_motion-4.0.0/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     2742 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    41645 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    24838 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    10610 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/io_port_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    17411 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      268 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope_data_source.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/pvt_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      256 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/pvt_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/pvt_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      247 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/pvt_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/pvt_sequence.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    76318 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.887053 zaber_motion-4.0.0/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.896158 zaber_motion-4.0.0/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_pvt_point.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      326 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      285 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.897335 zaber_motion-4.0.0/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1631 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.897569 zaber_motion-4.0.0/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.897941 zaber_motion-4.0.0/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    66351 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   202292 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     9021 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-06-05 20:44:42.000000 zaber_motion-4.0.0/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-05 20:45:30.879806 zaber_motion-4.0.0/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-05 20:45:30.000000 zaber_motion-4.0.0/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     7670 2023-06-05 20:45:30.000000 zaber_motion-4.0.0/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-06-05 20:45:30.000000 zaber_motion-4.0.0/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-06-05 20:45:30.000000 zaber_motion-4.0.0/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-05 20:45:30.000000 zaber_motion-4.0.0/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.481835 zaber_motion-4.2.0/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-17 02:49:41.481904 zaber_motion-4.2.0/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-06-17 02:49:41.482156 zaber_motion-4.2.0/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.458952 zaber_motion-4.2.0/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.460904 zaber_motion-4.2.0/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.467797 zaber_motion-4.2.0/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     2742 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    41645 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24838 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/io_port_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      268 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_data_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.469576 zaber_motion-4.2.0/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.479734 zaber_motion-4.2.0/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      396 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.480984 zaber_motion-4.2.0/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1631 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.481223 zaber_motion-4.2.0/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.481603 zaber_motion-4.2.0/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    66434 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   202637 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     9021 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.461476 zaber_motion-4.2.0/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7670 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-4.0.0/LICENSE.txt` & `zaber_motion-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/PKG-INFO` & `zaber_motion-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 4.0.0
+Version: 4.2.0
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.0.0/setup.py` & `zaber_motion-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='4.0.0',
+    version='4.2.0',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.8',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==4.0.0;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==4.0.0;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==4.0.0;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==4.2.0;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==4.2.0;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==4.2.0;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-4.0.0/test/test_integration.py` & `zaber_motion-4.2.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/__init__.py` & `zaber_motion-4.2.0/zaber_motion/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/__init__.py` & `zaber_motion-4.2.0/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/alert_event.py` & `zaber_motion-4.2.0/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/all_axes.py` & `zaber_motion-4.2.0/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/axis.py` & `zaber_motion-4.2.0/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/axis_identity.py` & `zaber_motion-4.2.0/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/axis_settings.py` & `zaber_motion-4.2.0/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/connection.py` & `zaber_motion-4.2.0/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-4.2.0/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/device.py` & `zaber_motion-4.2.0/zaber_motion/ascii/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/device_identity.py` & `zaber_motion-4.2.0/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/device_io.py` & `zaber_motion-4.2.0/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/device_io_info.py` & `zaber_motion-4.2.0/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/device_settings.py` & `zaber_motion-4.2.0/zaber_motion/ascii/device_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
 from ..units import UnitsAndLiterals, Units, units_from_literals
 
 if TYPE_CHECKING:
     from .device import Device
@@ -315,7 +315,51 @@
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
         response = main_pb2.BoolResponse()
         call_sync("device/can_convert_setting", request, response)
         return response.value
+
+    def get_from_all_axes(
+            self,
+            setting: str
+    ) -> List[float]:
+        """
+        Gets the value of an axis scope setting for each axis on the device.
+        Values may be NaN where the setting is not applicable.
+
+        Args:
+            setting: Name of the setting.
+
+        Returns:
+            The setting values on each axis.
+        """
+        request = main_pb2.DeviceGetSettingRequest()
+        request.interface_id = self._device.connection.interface_id
+        request.device = self._device.device_address
+        request.setting = setting
+        response = main_pb2.DoubleArrayResponse()
+        call("device/get_setting_from_all_axes", request, response)
+        return list(response.values)
+
+    async def get_from_all_axes_async(
+            self,
+            setting: str
+    ) -> List[float]:
+        """
+        Gets the value of an axis scope setting for each axis on the device.
+        Values may be NaN where the setting is not applicable.
+
+        Args:
+            setting: Name of the setting.
+
+        Returns:
+            The setting values on each axis.
+        """
+        request = main_pb2.DeviceGetSettingRequest()
+        request.interface_id = self._device.connection.interface_id
+        request.device = self._device.device_address
+        request.setting = setting
+        response = main_pb2.DoubleArrayResponse()
+        await call_async("device/get_setting_from_all_axes", request, response)
+        return list(response.values)
```

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/lockstep.py` & `zaber_motion-4.2.0/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-4.2.0/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     def add_io_channel(
             self,
             io_type: IoPortType,
             io_channel: int
     ) -> None:
         """
         Select an I/O pin to be recorded.
+        Requires at least Firmware 7.33.
 
         Args:
             io_type: The I/O port type to read data from.
             io_channel: The 1-based index of the I/O pin to read from.
         """
         request = main_pb2.OscilloscopeAddIoChannelRequest()
         request.interface_id = self.device.connection.interface_id
@@ -88,14 +89,15 @@
     async def add_io_channel_async(
             self,
             io_type: IoPortType,
             io_channel: int
     ) -> None:
         """
         Select an I/O pin to be recorded.
+        Requires at least Firmware 7.33.
 
         Args:
             io_type: The I/O port type to read data from.
             io_channel: The 1-based index of the I/O pin to read from.
         """
         request = main_pb2.OscilloscopeAddIoChannelRequest()
         request.interface_id = self.device.connection.interface_id
```

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/paramset_info.py` & `zaber_motion-4.2.0/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-4.2.0/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-4.2.0/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-4.2.0/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-4.2.0/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/response.py` & `zaber_motion-4.2.0/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-4.2.0/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-4.2.0/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/setting_constants.py` & `zaber_motion-4.2.0/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-4.2.0/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/storage.py` & `zaber_motion-4.2.0/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/stream.py` & `zaber_motion-4.2.0/zaber_motion/ascii/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,18 +463,18 @@
     ) -> None:
         """
         Queue an absolute arc movement on the first two axes of the stream.
         Absolute meaning that the home positions of the axes is treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.ABS
         request.rotation_direction = rotation_direction.value
@@ -494,18 +494,18 @@
     ) -> None:
         """
         Queue an absolute arc movement on the first two axes of the stream.
         Absolute meaning that the home positions of the axes is treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.ABS
         request.rotation_direction = rotation_direction.value
@@ -525,18 +525,18 @@
     ) -> None:
         """
         Queue a relative arc movement on the first two axes of the stream.
         Relative meaning that the current position of the axes is treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.REL
         request.rotation_direction = rotation_direction.value
@@ -556,18 +556,18 @@
     ) -> None:
         """
         Queue a relative arc movement on the first two axes of the stream.
         Relative meaning that the current position of the axes is treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.REL
         request.rotation_direction = rotation_direction.value
@@ -592,18 +592,18 @@
         Requires at least Firmware 7.11.
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.ABS
         request.target_axes_indices.extend(target_axes_indices)
@@ -629,18 +629,18 @@
         Requires at least Firmware 7.11.
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.ABS
         request.target_axes_indices.extend(target_axes_indices)
@@ -666,18 +666,18 @@
         Requires at least Firmware 7.11.
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.REL
         request.target_axes_indices.extend(target_axes_indices)
@@ -703,32 +703,196 @@
         Requires at least Firmware 7.11.
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
-            center_x: The first dimensions of the position of the center of the circle on which the arc exists.
-            center_y: The second dimensions of the position of the center of the circle on which the arc exists.
-            end_x: The first dimensions of the end position of the arc.
-            end_y: The second dimensions of the end position of the arc.
+            center_x: The first dimension of the position of the center of the circle on which the arc exists.
+            center_y: The second dimension of the position of the center of the circle on which the arc exists.
+            end_x: The first dimension of the end position of the arc.
+            end_y: The second dimension of the end position of the arc.
         """
         request = main_pb2.StreamArcRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.type = main_pb2.StreamArcRequest.REL
         request.target_axes_indices.extend(target_axes_indices)
         request.rotation_direction = rotation_direction.value
         request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
         request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
         request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
         request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
         await call_async("device/stream_arc", request)
 
+    def helix_absolute_on(
+            self,
+            target_axes_indices: List[int],
+            rotation_direction: RotationDirection,
+            center_x: Measurement,
+            center_y: Measurement,
+            end_x: Measurement,
+            end_y: Measurement,
+            *endpoint: Measurement
+    ) -> None:
+        """
+        Queue an absolute helix movement in the stream.
+        Requires at least Firmware 7.28.
+
+        Args:
+            target_axes_indices: Indices of the axes in the stream the movement targets.
+                Refers to the axes provided during the stream setup or further execution.
+                Indices are zero-based.
+                The first two axes refer to the helix's arc component,
+                while the rest refers to the helix's line component.
+            rotation_direction: The direction of the rotation.
+            center_x: The first dimension of the position of the center of the circle on which the helix projects.
+            center_y: The second dimension of the position of the center of the circle on which the helix projects.
+            end_x: The first dimension of the end position of the helix's arc component.
+            end_y: The second dimension of the end position of the helix's arc component.
+            endpoint: Positions for the helix's line component axes, relative to their home positions.
+        """
+        request = main_pb2.StreamArcRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.stream_id = self.stream_id
+        request.type = main_pb2.StreamArcRequest.ABS
+        request.target_axes_indices.extend(target_axes_indices)
+        request.rotation_direction = rotation_direction.value
+        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
+        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
+        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        call("device/stream_helix", request)
+
+    async def helix_absolute_on_async(
+            self,
+            target_axes_indices: List[int],
+            rotation_direction: RotationDirection,
+            center_x: Measurement,
+            center_y: Measurement,
+            end_x: Measurement,
+            end_y: Measurement,
+            *endpoint: Measurement
+    ) -> None:
+        """
+        Queue an absolute helix movement in the stream.
+        Requires at least Firmware 7.28.
+
+        Args:
+            target_axes_indices: Indices of the axes in the stream the movement targets.
+                Refers to the axes provided during the stream setup or further execution.
+                Indices are zero-based.
+                The first two axes refer to the helix's arc component,
+                while the rest refers to the helix's line component.
+            rotation_direction: The direction of the rotation.
+            center_x: The first dimension of the position of the center of the circle on which the helix projects.
+            center_y: The second dimension of the position of the center of the circle on which the helix projects.
+            end_x: The first dimension of the end position of the helix's arc component.
+            end_y: The second dimension of the end position of the helix's arc component.
+            endpoint: Positions for the helix's line component axes, relative to their home positions.
+        """
+        request = main_pb2.StreamArcRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.stream_id = self.stream_id
+        request.type = main_pb2.StreamArcRequest.ABS
+        request.target_axes_indices.extend(target_axes_indices)
+        request.rotation_direction = rotation_direction.value
+        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
+        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
+        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        await call_async("device/stream_helix", request)
+
+    def helix_relative_on(
+            self,
+            target_axes_indices: List[int],
+            rotation_direction: RotationDirection,
+            center_x: Measurement,
+            center_y: Measurement,
+            end_x: Measurement,
+            end_y: Measurement,
+            *endpoint: Measurement
+    ) -> None:
+        """
+        Queue a relative helix movement in the stream.
+        Requires at least Firmware 7.28.
+
+        Args:
+            target_axes_indices: Indices of the axes in the stream the movement targets.
+                Refers to the axes provided during the stream setup or further execution.
+                Indices are zero-based.
+                The first two axes refer to the helix's arc component,
+                while the rest refers to the helix's line component.
+            rotation_direction: The direction of the rotation.
+            center_x: The first dimension of the position of the center of the circle on which the helix projects.
+            center_y: The second dimension of the position of the center of the circle on which the helix projects.
+            end_x: The first dimension of the end position of the helix's arc component.
+            end_y: The second dimension of the end position of the helix's arc component.
+            endpoint: Positions for the helix's line component axes, relative to their positions before movement.
+        """
+        request = main_pb2.StreamArcRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.stream_id = self.stream_id
+        request.type = main_pb2.StreamArcRequest.REL
+        request.target_axes_indices.extend(target_axes_indices)
+        request.rotation_direction = rotation_direction.value
+        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
+        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
+        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        call("device/stream_helix", request)
+
+    async def helix_relative_on_async(
+            self,
+            target_axes_indices: List[int],
+            rotation_direction: RotationDirection,
+            center_x: Measurement,
+            center_y: Measurement,
+            end_x: Measurement,
+            end_y: Measurement,
+            *endpoint: Measurement
+    ) -> None:
+        """
+        Queue a relative helix movement in the stream.
+        Requires at least Firmware 7.28.
+
+        Args:
+            target_axes_indices: Indices of the axes in the stream the movement targets.
+                Refers to the axes provided during the stream setup or further execution.
+                Indices are zero-based.
+                The first two axes refer to the helix's arc component,
+                while the rest refers to the helix's line component.
+            rotation_direction: The direction of the rotation.
+            center_x: The first dimension of the position of the center of the circle on which the helix projects.
+            center_y: The second dimension of the position of the center of the circle on which the helix projects.
+            end_x: The first dimension of the end position of the helix's arc component.
+            end_y: The second dimension of the end position of the helix's arc component.
+            endpoint: Positions for the helix's line component axes, relative to their positions before movement.
+        """
+        request = main_pb2.StreamArcRequest()
+        request.interface_id = self.device.connection.interface_id
+        request.device = self.device.device_address
+        request.stream_id = self.stream_id
+        request.type = main_pb2.StreamArcRequest.REL
+        request.target_axes_indices.extend(target_axes_indices)
+        request.rotation_direction = rotation_direction.value
+        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
+        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
+        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        await call_async("device/stream_helix", request)
+
     def circle_absolute(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement
     ) -> None:
         """
```

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-4.2.0/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-4.2.0/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/transport.py` & `zaber_motion-4.2.0/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-4.2.0/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/warning_flags.py` & `zaber_motion-4.2.0/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/ascii/warnings.py` & `zaber_motion-4.2.0/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/__init__.py` & `zaber_motion-4.2.0/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/binary_settings.py` & `zaber_motion-4.2.0/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/command_code.py` & `zaber_motion-4.2.0/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/connection.py` & `zaber_motion-4.2.0/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/device.py` & `zaber_motion-4.2.0/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/device_identity.py` & `zaber_motion-4.2.0/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/device_settings.py` & `zaber_motion-4.2.0/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/error_code.py` & `zaber_motion-4.2.0/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/message.py` & `zaber_motion-4.2.0/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/reply_only_event.py` & `zaber_motion-4.2.0/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-4.2.0/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/bindings.py` & `zaber_motion-4.2.0/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/call.py` & `zaber_motion-4.2.0/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/convert_exception.py` & `zaber_motion-4.2.0/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/events.py` & `zaber_motion-4.2.0/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/__init__.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/firmware_version.py` & `zaber_motion-4.2.0/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/__init__.py` & `zaber_motion-4.2.0/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/axis_definition.py` & `zaber_motion-4.2.0/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-4.2.0/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-4.2.0/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/device_definition.py` & `zaber_motion-4.2.0/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/offline_translator.py` & `zaber_motion-4.2.0/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/translate_message.py` & `zaber_motion-4.2.0/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/translate_result.py` & `zaber_motion-4.2.0/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/translator.py` & `zaber_motion-4.2.0/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/gcode/translator_config.py` & `zaber_motion-4.2.0/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/library.py` & `zaber_motion-4.2.0/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/measurement.py` & `zaber_motion-4.2.0/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-4.2.0/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xbe\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protobufs.main_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\"./protobufs;zaber_motion_protobufs'
-  _MESSAGETYPE._serialized_start=22335
-  _MESSAGETYPE._serialized_end=22380
-  _ERRORS._serialized_start=22383
-  _ERRORS._serialized_end=23599
-  _INTERFACETYPE._serialized_start=23601
-  _INTERFACETYPE._serialized_end=23682
+  _MESSAGETYPE._serialized_start=22390
+  _MESSAGETYPE._serialized_end=22435
+  _ERRORS._serialized_start=22438
+  _ERRORS._serialized_end=23654
+  _INTERFACETYPE._serialized_start=23656
+  _INTERFACETYPE._serialized_end=23737
   _REQUEST._serialized_start=48
   _REQUEST._serialized_end=74
   _RESPONSE._serialized_start=77
   _RESPONSE._serialized_end=262
   _RESPONSE_RESPONSETYPE._serialized_start=229
   _RESPONSE_RESPONSETYPE._serialized_end=262
   _EVENT._serialized_start=264
@@ -260,197 +260,197 @@
   _PVTPOINTREQUEST_TYPE._serialized_start=11353
   _PVTPOINTREQUEST_TYPE._serialized_end=11377
   _STREAMLINEREQUEST._serialized_start=11380
   _STREAMLINEREQUEST._serialized_end=11641
   _STREAMLINEREQUEST_TYPE._serialized_start=11353
   _STREAMLINEREQUEST_TYPE._serialized_end=11377
   _STREAMARCREQUEST._serialized_start=11644
-  _STREAMARCREQUEST._serialized_end=12090
+  _STREAMARCREQUEST._serialized_end=12145
   _STREAMARCREQUEST_TYPE._serialized_start=11353
   _STREAMARCREQUEST_TYPE._serialized_end=11377
-  _STREAMCIRCLEREQUEST._serialized_start=12093
-  _STREAMCIRCLEREQUEST._serialized_end=12441
+  _STREAMCIRCLEREQUEST._serialized_start=12148
+  _STREAMCIRCLEREQUEST._serialized_end=12496
   _STREAMCIRCLEREQUEST_TYPE._serialized_start=11353
   _STREAMCIRCLEREQUEST_TYPE._serialized_end=11377
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12444
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12584
-  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12587
-  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12745
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12748
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=12888
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=12891
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=13030
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=13033
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=13161
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=13163
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=13284
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=13286
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13406
-  _STREAMWAITREQUEST._serialized_start=13408
-  _STREAMWAITREQUEST._serialized_end=13525
-  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13528
-  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13656
-  _STREAMEMPTYREQUEST._serialized_start=13658
-  _STREAMEMPTYREQUEST._serialized_end=13748
-  _STREAMGETAXESRESPONSE._serialized_start=13750
-  _STREAMGETAXESRESPONSE._serialized_end=13833
-  _STREAMGETMAXSPEEDREQUEST._serialized_start=13835
-  _STREAMGETMAXSPEEDREQUEST._serialized_end=13945
-  _STREAMSETMAXSPEEDREQUEST._serialized_start=13948
-  _STREAMSETMAXSPEEDREQUEST._serialized_end=14077
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14079
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14206
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14209
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14373
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14376
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14504
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14507
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14673
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14675
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14776
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14778
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=14832
-  _STREAMBUFFERERASEREQUEST._serialized_start=14834
-  _STREAMBUFFERERASEREQUEST._serialized_end=14930
-  _STREAMGENERICCOMMANDREQUEST._serialized_start=14932
-  _STREAMGENERICCOMMANDREQUEST._serialized_end=15048
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=15050
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=15169
-  _BINARYREPLYONLYEVENT._serialized_start=15171
-  _BINARYREPLYONLYEVENT._serialized_end=15270
-  _OPENBINARYINTERFACEREQUEST._serialized_start=15273
-  _OPENBINARYINTERFACEREQUEST._serialized_end=15460
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15462
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15567
-  _GENERICBINARYREQUEST._serialized_start=15570
-  _GENERICBINARYREQUEST._serialized_end=15700
-  _BINARYMESSAGE._serialized_start=15702
-  _BINARYMESSAGE._serialized_end=15772
-  _BINARYMESSAGECOLLECTION._serialized_start=15774
-  _BINARYMESSAGECOLLECTION._serialized_end=15856
-  _DEVICEEMPTYREQUEST._serialized_start=15858
-  _DEVICEEMPTYREQUEST._serialized_end=15916
-  _BINARYDEVICEIDENTITY._serialized_start=15919
-  _BINARYDEVICEIDENTITY._serialized_end=16264
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=16215
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=16264
-  _BINARYGENERICWITHUNITSREQUEST._serialized_start=16267
-  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16420
-  _BINARYDEVICEHOMEREQUEST._serialized_start=16422
-  _BINARYDEVICEHOMEREQUEST._serialized_end=16516
-  _BINARYDEVICEMOVEREQUEST._serialized_start=16519
-  _BINARYDEVICEMOVEREQUEST._serialized_end=16737
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12499
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12639
+  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12642
+  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12800
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12803
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=12943
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=12946
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=13085
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=13088
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=13216
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=13218
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=13339
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=13341
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13461
+  _STREAMWAITREQUEST._serialized_start=13463
+  _STREAMWAITREQUEST._serialized_end=13580
+  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13583
+  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13711
+  _STREAMEMPTYREQUEST._serialized_start=13713
+  _STREAMEMPTYREQUEST._serialized_end=13803
+  _STREAMGETAXESRESPONSE._serialized_start=13805
+  _STREAMGETAXESRESPONSE._serialized_end=13888
+  _STREAMGETMAXSPEEDREQUEST._serialized_start=13890
+  _STREAMGETMAXSPEEDREQUEST._serialized_end=14000
+  _STREAMSETMAXSPEEDREQUEST._serialized_start=14003
+  _STREAMSETMAXSPEEDREQUEST._serialized_end=14132
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14134
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14261
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14264
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14428
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14431
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14559
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14562
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14728
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14730
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14831
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14833
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=14887
+  _STREAMBUFFERERASEREQUEST._serialized_start=14889
+  _STREAMBUFFERERASEREQUEST._serialized_end=14985
+  _STREAMGENERICCOMMANDREQUEST._serialized_start=14987
+  _STREAMGENERICCOMMANDREQUEST._serialized_end=15103
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=15105
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=15224
+  _BINARYREPLYONLYEVENT._serialized_start=15226
+  _BINARYREPLYONLYEVENT._serialized_end=15325
+  _OPENBINARYINTERFACEREQUEST._serialized_start=15328
+  _OPENBINARYINTERFACEREQUEST._serialized_end=15515
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15517
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15622
+  _GENERICBINARYREQUEST._serialized_start=15625
+  _GENERICBINARYREQUEST._serialized_end=15755
+  _BINARYMESSAGE._serialized_start=15757
+  _BINARYMESSAGE._serialized_end=15827
+  _BINARYMESSAGECOLLECTION._serialized_start=15829
+  _BINARYMESSAGECOLLECTION._serialized_end=15911
+  _DEVICEEMPTYREQUEST._serialized_start=15913
+  _DEVICEEMPTYREQUEST._serialized_end=15971
+  _BINARYDEVICEIDENTITY._serialized_start=15974
+  _BINARYDEVICEIDENTITY._serialized_end=16319
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=16270
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=16319
+  _BINARYGENERICWITHUNITSREQUEST._serialized_start=16322
+  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16475
+  _BINARYDEVICEHOMEREQUEST._serialized_start=16477
+  _BINARYDEVICEHOMEREQUEST._serialized_end=16571
+  _BINARYDEVICEMOVEREQUEST._serialized_start=16574
+  _BINARYDEVICEMOVEREQUEST._serialized_end=16792
   _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5721
   _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5758
-  _BINARYDEVICESTOPREQUEST._serialized_start=16739
-  _BINARYDEVICESTOPREQUEST._serialized_end=16833
-  _BINARYDEVICEDETECTREQUEST._serialized_start=16835
-  _BINARYDEVICEDETECTREQUEST._serialized_end=16910
-  _BINARYDEVICEDETECTRESPONSE._serialized_start=16912
-  _BINARYDEVICEDETECTRESPONSE._serialized_end=16957
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=16959
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=17059
-  _BINARYDEVICESETSETTINGREQUEST._serialized_start=17061
-  _BINARYDEVICESETSETTINGREQUEST._serialized_end=17176
-  _CUSTOMINTERFACEREADREQUEST._serialized_start=17178
-  _CUSTOMINTERFACEREADREQUEST._serialized_end=17228
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=17230
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17298
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17300
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17351
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17353
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17427
-  _CANSETSTATEREQUEST._serialized_start=17429
-  _CANSETSTATEREQUEST._serialized_end=17516
-  _CANSETSTATEAXISRESPONSE._serialized_start=17518
-  _CANSETSTATEAXISRESPONSE._serialized_end=17579
-  _CANSETSTATEDEVICERESPONSE._serialized_start=17581
-  _CANSETSTATEDEVICERESPONSE._serialized_end=17693
-  _SETSTATEREQUEST._serialized_start=17695
-  _SETSTATEREQUEST._serialized_end=17800
-  _SERVOTUNINGREQUEST._serialized_start=17802
-  _SERVOTUNINGREQUEST._serialized_end=17892
-  _SERVOTUNINGPARAM._serialized_start=17894
-  _SERVOTUNINGPARAM._serialized_end=17941
-  _PARAMSETINFO._serialized_start=17943
-  _PARAMSETINFO._serialized_end=18046
-  _SETSERVOTUNINGREQUEST._serialized_start=18049
-  _SETSERVOTUNINGREQUEST._serialized_end=18207
-  _LOADPARAMSET._serialized_start=18209
-  _LOADPARAMSET._serialized_end=18319
-  _SETSERVOTUNINGPIDREQUEST._serialized_start=18322
-  _SETSERVOTUNINGPIDREQUEST._serialized_end=18463
-  _PIDTUNING._serialized_start=18465
-  _PIDTUNING._serialized_end=18552
-  _SETSIMPLETUNING._serialized_start=18555
-  _SETSIMPLETUNING._serialized_end=18749
-  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18751
-  _SIMPLETUNINGPARAMDEFINITION._serialized_end=18851
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=18853
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=18962
-  _TRANSLATORCREATEREQUEST._serialized_start=18965
-  _TRANSLATORCREATEREQUEST._serialized_end=19114
-  _TRANSLATORCREATERESPONSE._serialized_start=19116
-  _TRANSLATORCREATERESPONSE._serialized_end=19165
-  _TRANSLATORAXISDEFINITION._serialized_start=19167
-  _TRANSLATORAXISDEFINITION._serialized_end=19246
-  _TRANSLATORDEFINITION._serialized_start=19249
-  _TRANSLATORDEFINITION._serialized_end=19410
-  _TRANSLATORCONFIG._serialized_start=19413
-  _TRANSLATORCONFIG._serialized_end=19585
-  _TRANSLATORAXISMAPPING._serialized_start=19587
-  _TRANSLATORAXISMAPPING._serialized_end=19651
-  _TRANSLATORAXISTRANSFORMATION._serialized_start=19653
-  _TRANSLATORAXISTRANSFORMATION._serialized_end=19779
-  _TRANSLATORTRANSLATEREQUEST._serialized_start=19781
-  _TRANSLATORTRANSLATEREQUEST._serialized_end=19847
-  _TRANSLATEMESSAGE._serialized_start=19849
-  _TRANSLATEMESSAGE._serialized_end=19922
-  _TRANSLATORTRANSLATERESPONSE._serialized_start=19924
-  _TRANSLATORTRANSLATERESPONSE._serialized_end=20031
-  _GCODESYNTAXEXCEPTIONDATA._serialized_start=20033
-  _GCODESYNTAXEXCEPTIONDATA._serialized_end=20097
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=20099
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=20166
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=20168
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=20244
-  _TRANSLATORFLUSHRESPONSE._serialized_start=20246
-  _TRANSLATORFLUSHRESPONSE._serialized_end=20289
-  _TRANSLATORCREATELIVEREQUEST._serialized_start=20292
-  _TRANSLATORCREATELIVEREQUEST._serialized_end=20436
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20439
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20584
-  _TRANSLATOREMPTYREQUEST._serialized_start=20586
-  _TRANSLATOREMPTYREQUEST._serialized_end=20633
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20635
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20729
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20731
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=20834
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=20836
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=20921
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=20923
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=21033
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=21035
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=21117
-  _DEVICESETSTORAGEREQUEST._serialized_start=21119
-  _DEVICESETSTORAGEREQUEST._serialized_end=21240
-  _DEVICEGETSTORAGEREQUEST._serialized_start=21242
-  _DEVICEGETSTORAGEREQUEST._serialized_end=21348
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21350
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21461
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21463
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21572
-  _DEVICESTORAGEREQUEST._serialized_start=21574
-  _DEVICESTORAGEREQUEST._serialized_end=21661
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21663
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21761
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21764
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=21925
-  _CONVERSIONFACTOR._serialized_start=21927
-  _CONVERSIONFACTOR._serialized_end=21991
-  _OBJECTIVECHANGERREQUEST._serialized_start=21993
-  _OBJECTIVECHANGERREQUEST._serialized_end=22087
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22089
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22152
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22155
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22333
+  _BINARYDEVICESTOPREQUEST._serialized_start=16794
+  _BINARYDEVICESTOPREQUEST._serialized_end=16888
+  _BINARYDEVICEDETECTREQUEST._serialized_start=16890
+  _BINARYDEVICEDETECTREQUEST._serialized_end=16965
+  _BINARYDEVICEDETECTRESPONSE._serialized_start=16967
+  _BINARYDEVICEDETECTRESPONSE._serialized_end=17012
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=17014
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=17114
+  _BINARYDEVICESETSETTINGREQUEST._serialized_start=17116
+  _BINARYDEVICESETSETTINGREQUEST._serialized_end=17231
+  _CUSTOMINTERFACEREADREQUEST._serialized_start=17233
+  _CUSTOMINTERFACEREADREQUEST._serialized_end=17283
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=17285
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17353
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17355
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17406
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17408
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17482
+  _CANSETSTATEREQUEST._serialized_start=17484
+  _CANSETSTATEREQUEST._serialized_end=17571
+  _CANSETSTATEAXISRESPONSE._serialized_start=17573
+  _CANSETSTATEAXISRESPONSE._serialized_end=17634
+  _CANSETSTATEDEVICERESPONSE._serialized_start=17636
+  _CANSETSTATEDEVICERESPONSE._serialized_end=17748
+  _SETSTATEREQUEST._serialized_start=17750
+  _SETSTATEREQUEST._serialized_end=17855
+  _SERVOTUNINGREQUEST._serialized_start=17857
+  _SERVOTUNINGREQUEST._serialized_end=17947
+  _SERVOTUNINGPARAM._serialized_start=17949
+  _SERVOTUNINGPARAM._serialized_end=17996
+  _PARAMSETINFO._serialized_start=17998
+  _PARAMSETINFO._serialized_end=18101
+  _SETSERVOTUNINGREQUEST._serialized_start=18104
+  _SETSERVOTUNINGREQUEST._serialized_end=18262
+  _LOADPARAMSET._serialized_start=18264
+  _LOADPARAMSET._serialized_end=18374
+  _SETSERVOTUNINGPIDREQUEST._serialized_start=18377
+  _SETSERVOTUNINGPIDREQUEST._serialized_end=18518
+  _PIDTUNING._serialized_start=18520
+  _PIDTUNING._serialized_end=18607
+  _SETSIMPLETUNING._serialized_start=18610
+  _SETSIMPLETUNING._serialized_end=18804
+  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18806
+  _SIMPLETUNINGPARAMDEFINITION._serialized_end=18906
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=18908
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=19017
+  _TRANSLATORCREATEREQUEST._serialized_start=19020
+  _TRANSLATORCREATEREQUEST._serialized_end=19169
+  _TRANSLATORCREATERESPONSE._serialized_start=19171
+  _TRANSLATORCREATERESPONSE._serialized_end=19220
+  _TRANSLATORAXISDEFINITION._serialized_start=19222
+  _TRANSLATORAXISDEFINITION._serialized_end=19301
+  _TRANSLATORDEFINITION._serialized_start=19304
+  _TRANSLATORDEFINITION._serialized_end=19465
+  _TRANSLATORCONFIG._serialized_start=19468
+  _TRANSLATORCONFIG._serialized_end=19640
+  _TRANSLATORAXISMAPPING._serialized_start=19642
+  _TRANSLATORAXISMAPPING._serialized_end=19706
+  _TRANSLATORAXISTRANSFORMATION._serialized_start=19708
+  _TRANSLATORAXISTRANSFORMATION._serialized_end=19834
+  _TRANSLATORTRANSLATEREQUEST._serialized_start=19836
+  _TRANSLATORTRANSLATEREQUEST._serialized_end=19902
+  _TRANSLATEMESSAGE._serialized_start=19904
+  _TRANSLATEMESSAGE._serialized_end=19977
+  _TRANSLATORTRANSLATERESPONSE._serialized_start=19979
+  _TRANSLATORTRANSLATERESPONSE._serialized_end=20086
+  _GCODESYNTAXEXCEPTIONDATA._serialized_start=20088
+  _GCODESYNTAXEXCEPTIONDATA._serialized_end=20152
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=20154
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=20221
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=20223
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=20299
+  _TRANSLATORFLUSHRESPONSE._serialized_start=20301
+  _TRANSLATORFLUSHRESPONSE._serialized_end=20344
+  _TRANSLATORCREATELIVEREQUEST._serialized_start=20347
+  _TRANSLATORCREATELIVEREQUEST._serialized_end=20491
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20494
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20639
+  _TRANSLATOREMPTYREQUEST._serialized_start=20641
+  _TRANSLATOREMPTYREQUEST._serialized_end=20688
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20690
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20784
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20786
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=20889
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=20891
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=20976
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=20978
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=21088
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=21090
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=21172
+  _DEVICESETSTORAGEREQUEST._serialized_start=21174
+  _DEVICESETSTORAGEREQUEST._serialized_end=21295
+  _DEVICEGETSTORAGEREQUEST._serialized_start=21297
+  _DEVICEGETSTORAGEREQUEST._serialized_end=21403
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21405
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21516
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21518
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21627
+  _DEVICESTORAGEREQUEST._serialized_start=21629
+  _DEVICESTORAGEREQUEST._serialized_end=21716
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21718
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21816
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21819
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=21980
+  _CONVERSIONFACTOR._serialized_start=21982
+  _CONVERSIONFACTOR._serialized_end=22046
+  _OBJECTIVECHANGERREQUEST._serialized_start=22048
+  _OBJECTIVECHANGERREQUEST._serialized_end=22142
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22144
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22207
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22210
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22388
 # @@protoc_insertion_point(module_scope)
```

### Comparing `zaber_motion-4.0.0/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1969,14 +1969,15 @@
 
 global___SetLogOutputRequest = SetLogOutputRequest
 
 @typing_extensions.final
 class DeviceGetSettingRequest(google.protobuf.message.Message):
     """device/get_axis_setting
     device/get_axis_setting_str
+    device/get_setting_from_all_axes
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     AXIS_FIELD_NUMBER: builtins.int
@@ -2978,15 +2979,17 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "endpoint", b"endpoint", "interface_id", b"interface_id", "pvt", b"pvt", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
 
 global___StreamLineRequest = StreamLineRequest
 
 @typing_extensions.final
 class StreamArcRequest(google.protobuf.message.Message):
-    """device/stream_arc"""
+    """device/stream_arc
+    device/stream_helix
+    """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -3006,14 +3009,15 @@
     TYPE_FIELD_NUMBER: builtins.int
     ROTATION_DIRECTION_FIELD_NUMBER: builtins.int
     CENTER_X_FIELD_NUMBER: builtins.int
     CENTER_Y_FIELD_NUMBER: builtins.int
     END_X_FIELD_NUMBER: builtins.int
     END_Y_FIELD_NUMBER: builtins.int
     TARGET_AXES_INDICES_FIELD_NUMBER: builtins.int
+    ENDPOINT_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     device: builtins.int
     stream_id: builtins.int
     pvt: builtins.bool
     type: global___StreamArcRequest.Type.ValueType
     rotation_direction: builtins.int
     @property
@@ -3022,31 +3026,34 @@
     def center_y(self) -> global___Measurement: ...
     @property
     def end_x(self) -> global___Measurement: ...
     @property
     def end_y(self) -> global___Measurement: ...
     @property
     def target_axes_indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def endpoint(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Measurement]: ...
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         device: builtins.int = ...,
         stream_id: builtins.int = ...,
         pvt: builtins.bool = ...,
         type: global___StreamArcRequest.Type.ValueType = ...,
         rotation_direction: builtins.int = ...,
         center_x: global___Measurement | None = ...,
         center_y: global___Measurement | None = ...,
         end_x: global___Measurement | None = ...,
         end_y: global___Measurement | None = ...,
         target_axes_indices: collections.abc.Iterable[builtins.int] | None = ...,
+        endpoint: collections.abc.Iterable[global___Measurement] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "end_x", b"end_x", "end_y", b"end_y"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "device", b"device", "end_x", b"end_x", "end_y", b"end_y", "interface_id", b"interface_id", "pvt", b"pvt", "rotation_direction", b"rotation_direction", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["center_x", b"center_x", "center_y", b"center_y", "device", b"device", "end_x", b"end_x", "end_y", b"end_y", "endpoint", b"endpoint", "interface_id", b"interface_id", "pvt", b"pvt", "rotation_direction", b"rotation_direction", "stream_id", b"stream_id", "target_axes_indices", b"target_axes_indices", "type", b"type"]) -> None: ...
 
 global___StreamArcRequest = StreamArcRequest
 
 @typing_extensions.final
 class StreamCircleRequest(google.protobuf.message.Message):
     """device/stream_circle"""
```

### Comparing `zaber_motion-4.0.0/zaber_motion/serialization.py` & `zaber_motion-4.2.0/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/tools.py` & `zaber_motion-4.2.0/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion/units.py` & `zaber_motion-4.2.0/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.0.0/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-4.2.0/zaber_motion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 4.0.0
+Version: 4.2.0
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.0.0/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-4.2.0/zaber_motion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

