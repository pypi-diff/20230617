# Comparing `tmp/unitsnet-py-0.1.40.tar.gz` & `tmp/unitsnet-py-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitsnet-py-0.1.40.tar", last modified: Fri Jun 16 22:13:42 2023, max compression
+gzip compressed data, was "unitsnet-py-0.1.41.tar", last modified: Sat Jun 17 00:53:10 2023, max compression
```

## Comparing `unitsnet-py-0.1.40.tar` & `unitsnet-py-0.1.41.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:13:42.764318 unitsnet-py-0.1.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 22:12:52.000000 unitsnet-py-0.1.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-06-16 22:13:42.764318 unitsnet-py-0.1.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27204 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-16 22:13:37.000000 unitsnet-py-0.1.40/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:13:42.764318 unitsnet-py-0.1.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 22:13:37.000000 unitsnet-py-0.1.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:13:42.748318 unitsnet-py-0.1.40/unitsnet_py/
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:13:42.764318 unitsnet-py-0.1.40/unitsnet_py/units/
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/amount_of_substance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/amplitude_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/apparent_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/apparent_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/area_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/area_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/brake_specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/capacitance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/coefficient_of_thermal_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/compressibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/density.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/dynamic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_admittance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_conductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_current_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_current_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_inductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-16 22:13:33.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_potential_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_potential_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_potential_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_resistivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/electric_surface_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/energy_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/force_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/force_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/fuel_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/heat_transfer_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/information.py
--rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/irradiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/jerk.py
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/kinematic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/leak_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    50654 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/linear_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/linear_power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/luminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/luminous_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/luminous_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/magnetic_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/magnetic_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/mass_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/mass_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/mass_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/mass_fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/mass_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/molar_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/molar_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/molar_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/molar_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/molarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/permittivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/porous_medium_permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/power.py
--rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/power_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)    28785 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/pressure_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/ratio_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/reactive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/reactive_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/reciprocal_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/reciprocal_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/relative_humidity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/rotational_acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/rotational_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-06-16 22:13:34.000000 unitsnet-py-0.1.40/unitsnet_py/units/rotational_stiffness.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/rotational_stiffness_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/solid_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/specific_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/specific_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/specific_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/specific_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/standard_volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/temperature_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/temperature_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/temperature_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/thermal_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/torque_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/turbidity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/vitamin_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/volume_flow_per_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/volume_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/volumetric_heat_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-16 22:13:35.000000 unitsnet-py-0.1.40/unitsnet_py/units/warping_moment_of_inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:13:42.748318 unitsnet-py-0.1.40/unitsnet_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-06-16 22:13:42.000000 unitsnet-py-0.1.40/unitsnet_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-16 22:13:42.000000 unitsnet-py-0.1.40/unitsnet_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:13:42.000000 unitsnet-py-0.1.40/unitsnet_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 22:13:42.000000 unitsnet-py-0.1.40/unitsnet_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:53:10.140156 unitsnet-py-0.1.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 00:52:31.000000 unitsnet-py-0.1.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-06-17 00:53:10.140156 unitsnet-py-0.1.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27204 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-17 00:53:03.000000 unitsnet-py-0.1.41/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 00:53:10.140156 unitsnet-py-0.1.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-17 00:53:04.000000 unitsnet-py-0.1.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:53:10.128156 unitsnet-py-0.1.41/unitsnet_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:53:10.140156 unitsnet-py-0.1.41/unitsnet_py/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/amount_of_substance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/amplitude_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/apparent_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/apparent_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/area_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/area_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/brake_specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/capacitance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/coefficient_of_thermal_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/dynamic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_admittance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_conductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_current_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_current_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_inductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_potential_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_potential_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_potential_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_resistivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/electric_surface_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/energy_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/force_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/force_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/fuel_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/heat_transfer_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/jerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/kinematic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/leak_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50654 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/linear_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/linear_power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/luminous_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/luminous_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-17 00:53:00.000000 unitsnet-py-0.1.41/unitsnet_py/units/magnetic_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/magnetic_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/mass_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/mass_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/mass_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/mass_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/mass_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/molar_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/molar_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/molar_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/molar_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/molarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/permittivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/porous_medium_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/power_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28785 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/pressure_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/ratio_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/reactive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/reactive_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/reciprocal_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/reciprocal_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/relative_humidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/rotational_acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/rotational_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/rotational_stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/rotational_stiffness_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/specific_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/specific_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/specific_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/specific_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/standard_volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/temperature_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/temperature_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/temperature_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/thermal_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/torque_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/turbidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/vitamin_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/volume_flow_per_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/volume_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/volumetric_heat_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-17 00:53:01.000000 unitsnet-py-0.1.41/unitsnet_py/units/warping_moment_of_inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:53:10.128156 unitsnet-py-0.1.41/unitsnet_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-06-17 00:53:10.000000 unitsnet-py-0.1.41/unitsnet_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-17 00:53:10.000000 unitsnet-py-0.1.41/unitsnet_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:53:10.000000 unitsnet-py-0.1.41/unitsnet_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 00:53:10.000000 unitsnet-py-0.1.41/unitsnet_py.egg-info/top_level.txt
```

### Comparing `unitsnet-py-0.1.40/LICENSE` & `unitsnet-py-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/PKG-INFO` & `unitsnet-py-0.1.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.40
+Version: 0.1.41
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
```

### Comparing `unitsnet-py-0.1.40/README.md` & `unitsnet-py-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/pyproject.toml` & `unitsnet-py-0.1.41/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitsnet_py"
-version = "0.1.40"
+version = "0.1.41"
 description = "A better way to hold unit variables and easily convert to the destination unit"
 repository = "https://github.com/haimkastner/unitsnet-py"
 authors = ["Haim Kastner <haim.kastner@gmail.com>"]
 maintainers = [
     "Haim Kastner <haim.kastner@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `unitsnet-py-0.1.40/setup.py` & `unitsnet-py-0.1.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['unitsnet_py', 'unitsnet_py.units']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unitsnet-py',
-    'version': '0.1.40',
+    'version': '0.1.41',
     'keywords': 'conversion, units-of-measure, units, quantities, unit-converter, converter, unit, measure, measures, measurement, measurements',
     'description': 'A better way to hold unit variables and easily convert to the destination unit',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Haim Kastner',
     'author_email': 'haim.kastner@gmail.com',
     'maintainer': 'Haim Kastner',
```

### Comparing `unitsnet-py-0.1.40/unitsnet_py/__init__.py` & `unitsnet-py-0.1.41/unitsnet_py/__init__.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py` & `unitsnet-py-0.1.41/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/acceleration.py` & `unitsnet-py-0.1.41/unitsnet_py/units/acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/amount_of_substance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/amount_of_substance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/amplitude_ratio.py` & `unitsnet-py-0.1.41/unitsnet_py/units/amplitude_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/angle.py` & `unitsnet-py-0.1.41/unitsnet_py/units/angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/apparent_energy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/apparent_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/apparent_power.py` & `unitsnet-py-0.1.41/unitsnet_py/units/apparent_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/area.py` & `unitsnet-py-0.1.41/unitsnet_py/units/area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/area_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/area_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/area_moment_of_inertia.py` & `unitsnet-py-0.1.41/unitsnet_py/units/area_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/bit_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/bit_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/brake_specific_fuel_consumption.py` & `unitsnet-py-0.1.41/unitsnet_py/units/brake_specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/capacitance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/capacitance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/coefficient_of_thermal_expansion.py` & `unitsnet-py-0.1.41/unitsnet_py/units/coefficient_of_thermal_expansion.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/compressibility.py` & `unitsnet-py-0.1.41/unitsnet_py/units/compressibility.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/duration.py` & `unitsnet-py-0.1.41/unitsnet_py/units/duration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/dynamic_viscosity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/dynamic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_admittance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_admittance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_charge.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_charge.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_charge_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_conductance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_conductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_conductivity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_current.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_current.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_current_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_current_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_current_gradient.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_current_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_field.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_inductance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_inductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_potential.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_potential.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_potential_ac.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_potential_ac.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_potential_change_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_potential_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_potential_dc.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_potential_dc.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_resistance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_resistivity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_resistivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/electric_surface_charge_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/electric_surface_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/energy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/energy_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/energy_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/entropy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/force.py` & `unitsnet-py-0.1.41/unitsnet_py/units/force.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/force_change_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/force_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/force_per_length.py` & `unitsnet-py-0.1.41/unitsnet_py/units/force_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/frequency.py` & `unitsnet-py-0.1.41/unitsnet_py/units/frequency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/fuel_efficiency.py` & `unitsnet-py-0.1.41/unitsnet_py/units/fuel_efficiency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/heat_flux.py` & `unitsnet-py-0.1.41/unitsnet_py/units/heat_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/heat_transfer_coefficient.py` & `unitsnet-py-0.1.41/unitsnet_py/units/heat_transfer_coefficient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/illuminance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/illuminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/impulse.py` & `unitsnet-py-0.1.41/unitsnet_py/units/impulse.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/information.py` & `unitsnet-py-0.1.41/unitsnet_py/units/information.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/irradiance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/irradiance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/irradiation.py` & `unitsnet-py-0.1.41/unitsnet_py/units/irradiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/jerk.py` & `unitsnet-py-0.1.41/unitsnet_py/units/jerk.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/kinematic_viscosity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/kinematic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/leak_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/leak_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/length.py` & `unitsnet-py-0.1.41/unitsnet_py/units/length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/level.py` & `unitsnet-py-0.1.41/unitsnet_py/units/level.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/linear_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/linear_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/linear_power_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/linear_power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/luminance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/luminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/luminosity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/luminosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/luminous_flux.py` & `unitsnet-py-0.1.41/unitsnet_py/units/luminous_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/luminous_intensity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/luminous_intensity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/magnetic_field.py` & `unitsnet-py-0.1.41/unitsnet_py/units/magnetic_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/magnetic_flux.py` & `unitsnet-py-0.1.41/unitsnet_py/units/magnetic_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/magnetization.py` & `unitsnet-py-0.1.41/unitsnet_py/units/magnetization.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/mass.py` & `unitsnet-py-0.1.41/unitsnet_py/units/mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/mass_concentration.py` & `unitsnet-py-0.1.41/unitsnet_py/units/mass_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/mass_flow.py` & `unitsnet-py-0.1.41/unitsnet_py/units/mass_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/mass_flux.py` & `unitsnet-py-0.1.41/unitsnet_py/units/mass_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/mass_fraction.py` & `unitsnet-py-0.1.41/unitsnet_py/units/mass_fraction.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/mass_moment_of_inertia.py` & `unitsnet-py-0.1.41/unitsnet_py/units/mass_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/molar_energy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/molar_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/molar_entropy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/molar_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/molar_flow.py` & `unitsnet-py-0.1.41/unitsnet_py/units/molar_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/molar_mass.py` & `unitsnet-py-0.1.41/unitsnet_py/units/molar_mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/molarity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/molarity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/permeability.py` & `unitsnet-py-0.1.41/unitsnet_py/units/permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/permittivity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/permittivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/porous_medium_permeability.py` & `unitsnet-py-0.1.41/unitsnet_py/units/porous_medium_permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/power.py` & `unitsnet-py-0.1.41/unitsnet_py/units/power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/power_density.py` & `unitsnet-py-0.1.41/unitsnet_py/units/power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/power_ratio.py` & `unitsnet-py-0.1.41/unitsnet_py/units/power_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/pressure.py` & `unitsnet-py-0.1.41/unitsnet_py/units/pressure.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/pressure_change_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/pressure_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/ratio.py` & `unitsnet-py-0.1.41/unitsnet_py/units/ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/ratio_change_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/ratio_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/reactive_energy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/reactive_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/reactive_power.py` & `unitsnet-py-0.1.41/unitsnet_py/units/reactive_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/reciprocal_area.py` & `unitsnet-py-0.1.41/unitsnet_py/units/reciprocal_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/reciprocal_length.py` & `unitsnet-py-0.1.41/unitsnet_py/units/reciprocal_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/relative_humidity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/relative_humidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/rotational_acceleration.py` & `unitsnet-py-0.1.41/unitsnet_py/units/rotational_acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/rotational_speed.py` & `unitsnet-py-0.1.41/unitsnet_py/units/rotational_speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/rotational_stiffness.py` & `unitsnet-py-0.1.41/unitsnet_py/units/rotational_stiffness.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/rotational_stiffness_per_length.py` & `unitsnet-py-0.1.41/unitsnet_py/units/rotational_stiffness_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/scalar.py` & `unitsnet-py-0.1.41/unitsnet_py/units/scalar.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/solid_angle.py` & `unitsnet-py-0.1.41/unitsnet_py/units/solid_angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/specific_energy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/specific_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/specific_entropy.py` & `unitsnet-py-0.1.41/unitsnet_py/units/specific_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/specific_fuel_consumption.py` & `unitsnet-py-0.1.41/unitsnet_py/units/specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/specific_volume.py` & `unitsnet-py-0.1.41/unitsnet_py/units/specific_volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/specific_weight.py` & `unitsnet-py-0.1.41/unitsnet_py/units/specific_weight.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/speed.py` & `unitsnet-py-0.1.41/unitsnet_py/units/speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/standard_volume_flow.py` & `unitsnet-py-0.1.41/unitsnet_py/units/standard_volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/temperature.py` & `unitsnet-py-0.1.41/unitsnet_py/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/temperature_change_rate.py` & `unitsnet-py-0.1.41/unitsnet_py/units/temperature_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/temperature_delta.py` & `unitsnet-py-0.1.41/unitsnet_py/units/temperature_delta.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/temperature_gradient.py` & `unitsnet-py-0.1.41/unitsnet_py/units/temperature_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/thermal_conductivity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/thermal_resistance.py` & `unitsnet-py-0.1.41/unitsnet_py/units/thermal_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/torque.py` & `unitsnet-py-0.1.41/unitsnet_py/units/torque.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/torque_per_length.py` & `unitsnet-py-0.1.41/unitsnet_py/units/torque_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/turbidity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/turbidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/vitamin_a.py` & `unitsnet-py-0.1.41/unitsnet_py/units/vitamin_a.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/volume.py` & `unitsnet-py-0.1.41/unitsnet_py/units/volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/volume_concentration.py` & `unitsnet-py-0.1.41/unitsnet_py/units/volume_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/volume_flow.py` & `unitsnet-py-0.1.41/unitsnet_py/units/volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/volume_flow_per_area.py` & `unitsnet-py-0.1.41/unitsnet_py/units/volume_flow_per_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/volume_per_length.py` & `unitsnet-py-0.1.41/unitsnet_py/units/volume_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/volumetric_heat_capacity.py` & `unitsnet-py-0.1.41/unitsnet_py/units/volumetric_heat_capacity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py/units/warping_moment_of_inertia.py` & `unitsnet-py-0.1.41/unitsnet_py/units/warping_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.40/unitsnet_py.egg-info/PKG-INFO` & `unitsnet-py-0.1.41/unitsnet_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.40
+Version: 0.1.41
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
```

### Comparing `unitsnet-py-0.1.40/unitsnet_py.egg-info/SOURCES.txt` & `unitsnet-py-0.1.41/unitsnet_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

