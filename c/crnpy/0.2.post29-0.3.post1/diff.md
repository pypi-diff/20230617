# Comparing `tmp/crnpy-0.2.post29.tar.gz` & `tmp/crnpy-0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.2.post29.tar", last modified: Wed Jun  7 15:17:33 2023, max compression
+gzip compressed data, was "crnpy-0.3.post1.tar", last modified: Fri Jun 16 23:49:30 2023, max compression
```

## Comparing `crnpy-0.2.post29.tar` & `crnpy-0.3.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:17:33.398057 crnpy-0.2.post29/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 15:17:22.000000 crnpy-0.2.post29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-07 15:17:33.398057 crnpy-0.2.post29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-07 15:17:22.000000 crnpy-0.2.post29/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:17:33.398057 crnpy-0.2.post29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-07 15:17:22.000000 crnpy-0.2.post29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:17:33.398057 crnpy-0.2.post29/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:17:33.398057 crnpy-0.2.post29/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 15:17:22.000000 crnpy-0.2.post29/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43957 2023-06-07 15:17:22.000000 crnpy-0.2.post29/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-07 15:17:22.000000 crnpy-0.2.post29/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:17:33.398057 crnpy-0.2.post29/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-07 15:17:33.000000 crnpy-0.2.post29/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-07 15:17:33.000000 crnpy-0.2.post29/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:17:33.000000 crnpy-0.2.post29/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 15:17:33.000000 crnpy-0.2.post29/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 23:49:21.000000 crnpy-0.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.905187 crnpy-0.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-16 23:49:21.000000 crnpy-0.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:49:30.905187 crnpy-0.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 23:49:21.000000 crnpy-0.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.901188 crnpy-0.3.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53443 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.2.post29/LICENSE` & `crnpy-0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.2.post29/src/crnpy/crnpy.py` & `crnpy-0.3.post1/src/crnpy/crnpy.py`

 * *Files 14% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         2   98.0
         3   102.0
     """
 
     counts=counts.copy()
 
     if type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
-        warnings.warn("No count time columns provided. Using timestamp index to compute count time.")
+        print("No count time columns provided. Using timestamp index to compute count time.")
         count_times = counts.index.to_series().diff().dt.total_seconds()
 
     if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
         raise ValueError('Index must be a timestamp or count times must be provided.')
 
     if len(counts) != len(count_times):
         raise ValueError('Count times length does not match number of readings.')
@@ -231,15 +231,15 @@
     #Compute sum of counts
     total_raw_counts = counts.sum(axis=1)
     # Replace zeros with NaN
     total_raw_counts = total_raw_counts.replace(0, np.nan)
     return total_raw_counts
 
 
-def drop_outlier(raw_counts, window=5, store_outliers=False, min_counts=None, max_counts=None):
+def drop_outliers(raw_counts, window=5, store_outliers=False, min_counts=None, max_counts=None):
     """Computation of a moving modified Z-score based on the median absolute difference.
     
     Args:
         raw_counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         window (int): Window size for the moving median. Default is 11.
         store_outliers (bool): If True, store the outliers in a new column. Default is False.
         min_counts (int): Minimum number of counts for a reading to be considered valid. Default is None.
@@ -301,15 +301,25 @@
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.interpolate.html
     """
 
     # Fill missing values in atmospheric variables
     return cols_atm.interpolate(method='pchip', limit=limit, limit_direction='both')
 
 def atm_correction(raw_counts, pressure, humidity, temp, Pref, Aref, L, incoming_neutrons=None, incoming_Ref=None):
-    """Correct neutron counts for atmospheric factors and incoming neutron flux.
+    r"""Correct neutron counts for atmospheric factors and incoming neutron flux.
+
+    This function corrects neutron counts for atmospheric pressure, and absolute humidity using the method described in Zreda et al. (2012) and Anderson et al. (2017). The correction is performed using the following equation:
+
+    $$
+    C_{corrected} = \frac{C_{raw} \cdot f_w}{f_p \cdot f_i}
+    $$
+
+    - fp: pressure correction factor
+    - fw: abosolute humidity correction factor
+    - fi: incoming neutron flux correction factor
     
     Args:
         raw_counts (list or array): Neutron counts to correct.
         pressure (list or array): Atmospheric pressure readings.
         humidity (list or array): Atmospheric humidity readings in %.
         temp (list or array): Atmospheric temperature readings in Celsius.
         Pref (float): Reference atmospheric pressure in millibars (mbar).
@@ -359,37 +369,40 @@
         fi.fillna(1.0, inplace=True) # Use a value of 1 for days without data
 
     # Apply correction factors
     return np.round((raw_counts*fw)/(fp*fi))
 
 
 
-def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, verbose=False):
+def get_incoming_neutron_flux(start_date, end_date, station, utc_offset=0, expand_window = 0,  verbose=False):
     """Function to retrieve neutron flux from the Neutron Monitor Database.
 
     Args:
         start_date (datetime): Start date of the time series.
         end_date (datetime): End date of the time series.
         station (str): Neutron Monitor station to retrieve data from.
         utc_offset (int): UTC offset in hours. Default is 0.
+        expand_window (int): Number of hours to expand the time window to retrieve extra data. Default is 0.
         verbose (bool): Print information about the request. Default is False.
 
     Returns:
         (pandas.DataFrame): Neutron flux in counts per hour and timestamps.
 
     References:
         Documentation available:https://www.nmdb.eu/nest/help.php#howto
     """
 
     # Example: get_incoming_flux(station='IRKT',start_date='2020-04-10 11:00:00',end_date='2020-06-18 17:00:00')
     # Template url = 'http://nest.nmdb.eu/draw_graph.php?formchk=1&stations[]=KERG&output=ascii&tabchoice=revori&dtype=corr_for_efficiency&date_choice=bydate&start_year=2009&start_month=09&start_day=01&start_hour=00&start_min=00&end_year=2009&end_month=09&end_day=05&end_hour=23&end_min=59&yunits=0'
 
 
-    # Add 1 hour to ensure the last date is included in the request.
-    end_date += pd.Timedelta(hours=1)
+    # Expand the time window by 1 hour to ensure an extra observation is included in the request.
+    start_date -= pd.Timedelta(hours=expand_window)
+    end_date += pd.Timedelta(hours=expand_window)
+
 
     # Convert local time to UTC
     start_date = start_date - datetime.timedelta(hours=utc_offset)
     end_date = end_date - datetime.timedelta(hours=utc_offset)
     date_format = '%Y-%m-%d %H:%M:%S'
     root = 'http://www.nmdb.eu/nest/draw_graph.php?'
     url_par = [ 'formchk=1',
@@ -431,53 +444,57 @@
             print(f"Error retrieving data from {url}")
         return None
 
     # Check if all values from selected detector are NaN. If yes, warn the user
     if df_flux['counts'].isna().all():
         warnings.warn('Data for selected neutron detectors appears to be unavailable for the selected period')
 
+    # Convert timestamp to datetime and apply UTC offset
+    df_flux['timestamp'] = pd.to_datetime(df_flux['timestamp'])
+    df_flux['timestamp'] = df_flux['timestamp'] + pd.Timedelta(hours=utc_offset)
 
     # Print acknowledgement to inform users about restrictions and to acknowledge the NMDB database
     acknowledgement = """Data retrieved via NMDB are the property of the individual data providers. These data are free for non commercial
 use to within the restriction imposed by the providers. If you use such data for your research or applications, please acknowledge
 the origin by a sentence like 'We acknowledge the NMDB database (www.nmdb.eu) founded under the European Union's FP7 programme 
 (contract no. 213007), and the PIs of individual neutron monitors at: IGY Jungfraujoch 
 (Physikalisches Institut, University of Bern, Switzerland)"""
     #print(acknowledgement)
 
-    return df_flux
+    return df_flux.set_index('timestamp')
 
 def interpolate_incoming_flux(df_flux, timestamps):
-    """Function to interpolate incoming neutron flux.
+    """Function to interpolate incoming neutron flux to match the timestamps of the observations.
 
     Args:
         df_flux (pd.DataFrame): Dataframe returned by get_incoming_flux method.
         timestamps (pd.series or pd.DataFrame or pd.DatetimeIndex): Timestamps to interpolate the incoming neutron flux.
 
     Returns:
         (pd.DataFrame): Dataframe containing interpolated incoming neutron flux.
     """
 
-    # Add timestamps with nan values to the dataframe
-    df_flux['timestamp'] = pd.to_datetime(df_flux['timestamp'])
-    df_flux = df_flux.set_index('timestamp')
+    # Check that index is datetime
+    if not isinstance(df_flux.index, pd.DatetimeIndex):
+        raise ValueError('Index of df_flux must be datetime')
+
     for timestamp in timestamps:
         if timestamp not in df_flux.index:
             df_flux.loc[timestamp] = np.nan
     df_flux = df_flux.sort_index()
 
     # Interpolate nan values
-    df_flux = df_flux['counts'].interpolate(method='nearest')
+    df_flux = df_flux['counts'].interpolate(method='nearest', limit_direction='both')
 
     # Retur only the values for the selected timestamps
     return df_flux.loc[timestamps]
 
 
-def smooth_counts(corrected_counts,window=5,order=3, method='moving_median'):
-    """Use a Savitzky-Golay filter to smooth the signal of corrected neutron counts.
+def smooth_1D(corrected_counts,window=5,order=3, method='moving_median'):
+    """Use a Savitzky-Golay filter to smooth the signal of corrected neutron counts or another one-dimensional array (e.g. computed volumetric water content).
 
     Args:
         corrected_counts (pd.DataFrame): Dataframe containing the corrected neutron counts.
         window (int): Window size for the Savitzky-Golay filter. Default is 5.
         method (str): Method to use for smoothing the data. Default is 'moving_median'.
             Options are 'moving_average', 'moving_median' and 'savitzky_golay'.
         order (int): Order of the Savitzky-Golay filter. Default is 3.
@@ -579,17 +596,20 @@
     C_roads = 1 + F1 * F2 * F3
 
     corrected_counts = counts / C_roads
 
     return corrected_counts
 
 def counts_to_vwc(counts, N0, Wlat, Wsoc ,bulk_density, a0=0.0808,a1=0.372,a2=0.115):
-    """Function to convert corrected and filtered neutron counts into volumetric water content
-        following the approach described in Desilets et al., 2010.
-    
+    r"""Function to convert corrected and filtered neutron counts into volumetric water content.
+
+    This method implements soil moisture estimation using the non-linear relationship between neutron count and soil volumetric water content following the approach described in Desilets et al., 2010.
+
+    $\theta(N) =\frac{a_0}{(\frac{N}{N_0}) - a_1} - a_2 $
+
     Args:
         counts (array or pd.Series or pd.DataFrame): Array of corrected and filtered neutron counts.
         N0 (float): Device-specific neutron calibration constant.
         Wlat (float): Lattice water content.
         Wsoc (float): Soil organic carbon content.
         bulk_density (float): Soil bulk density.
         a0 (float): Parameter given in Zreda et al., 2012. Default is 0.0808.
@@ -607,15 +627,15 @@
 
     # Convert neutron counts into vwc
     vwc = (a0 / (counts/N0-a1) - a2 - Wlat - Wsoc) * bulk_density
     return vwc
 
 
 
-def sensing_depth(vwc, pressure, p_ref, bulk_density, Wlat, method='Schron_2017',dist=[0.5]):
+def sensing_depth(vwc, pressure, p_ref, bulk_density, Wlat, dist, method='Schron_2017'):
     # Convert docstring to google format
     """Function that computes the estimated sensing depth of the cosmic-ray neutron probe.
     The function offers several methods to compute the depth at which 86 % of the neutrons
     probes the soil profile.
 
     Args:
         vwc (array or pd.Series or pd.DataFrame): Estimated volumetric water content for each timestamp.
@@ -655,20 +675,45 @@
             results.append(D86)
 
     elif method == 'Franz_2012':
         results = [5.8/(bulk_density*Wlat+vwc+0.0829)]
 
     return results
 
+def estimate_abs_humidity(RH, temp):
+    """
+    Compute the actual vapor pressure (e) in g m^-3 using RH (%) and current temperature (c) observations.
+
+    Args:
+        RH (float): relative humidity (%)
+        temp (float): temperature (Celsius)
+
+    Returns:
+        float: actual vapor pressure (g m^-3)
+    """
+
+    ### Atmospheric water vapor factor
+    # Saturation vapor pressure
+    e_sat = 0.611 * np.exp(17.502 * temp / (
+                temp + 240.97)) * 1000  # in Pascals Eq. 3.8 p.41 Environmental Biophysics (Campbell and Norman)
+
+    # Vapor pressure Pascals
+    Pw = e_sat * RH / 100
+
+    # Absolute humidity (g/m^3)
+    C = 2.16679  # g K/J;
+    abs_h = C * Pw / (temp + 273.15)
+    return abs_h
+
 
 def nrad_weight(h,theta,distances,depth,rhob=1.4):
     """Function to compute distance weights corresponding to each soil sample.
 
     Args:
-        h (float): Air Humidity  from 0.1  to 50    in g/m^3. When h=0, the function will skip the distance weighting.
+        h (float): Air Humidity  from 0.1  to 50 in g/m^3. When h=0, the function will skip the distance weighting.
         theta (array or pd.Series or pd.DataFrame): Soil Moisture for each sample (0.02 - 0.50 m^3/m^3)
         distances (array or pd.Series or pd.DataFrame): Distances from the location of each sample to the origin (0.5 - 600 m)
         depth (array or pd.Series or pd.DataFrame): Depths for each sample (m)
         rhob (float): Bulk density in g/cm^3
 
     Returns:
         (array or pd.Series or pd.DataFrame): Distance weights for each sample.
@@ -729,77 +774,14 @@
 
     # Combined and normalized weights
     weights = Wd*W/np.nansum(Wd*W)
 
     return weights
 
 
-def haversine(lat1, lng1, lat2, lng2):
-    """Calculate the great circle distance between two points on the earth (specified in decimal degrees).
-
-    Args:
-        lat1 (float): Latitude of the first point.
-        lng1 (float): Longitude of the first point.
-        lat2 (float): Latitude of the second point.
-        lng2 (float): Longitude of the second point.
-
-    Returns:
-        (float): Distance between the two points in meters.
-
-    References:
-        https://en.wikipedia.org/wiki/Haversine_formula
-    """
-
-    # Convert decimal degrees to radians
-    lng1, lat1, lng2, lat2 = map(np.radians, [lng1, lat1, lng2, lat2])
-
-    # Haversine formula
-    dlng = lng2 - lng1
-    dlat = lat2 - lat1
-    a = np.sin(dlat/2)**2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlng/2)**2
-    c = 2 * np.arcsin(np.sqrt(a))
-
-    # Radius of earth in kilometers is 6371
-    km = 6371* c
-    return km*1000
-
-def spatial_smooth(sm, lat, lng, max_dist=500, min_neighbours=3):
-    # Convert the docstring to google-style
-    """Spatial smoothing of soil moisture data using inverse distance weighting.
-
-    Args:
-        sm (list or array): Soil moisture in mm of water.
-        lat (list or array): Latitude of the measurement points.
-        lng (list or array): Longitude of the measurement points.
-        max_dist (float): Maximum distance to consider for the spatial smoothing in meters.
-        min_neighbours (int): Minimum number of neighbours to consider for the spatial smoothing.
-        intensity (int): Intensity of the inverse distance weighting.
-
-    Returns:
-        (array): Spatially smoothed soil moisture in mm of water.
-
-    References:
-        Andres Patrignani. (2020). PyNotes for Environmental Scientists (v1.0). Zenodo. https://doi.org/10.5281/zenodo.3731390
-    """
-
-    sm_ini = np.array(sm)
-    sm_result = np.array(sm)
-
-    for i in range(len(lat)):
-        sm_i = np.array([])
-        for j in range(len(lat)):
-            dist = haversine(lat[i], lng[i], lat[j], lng[j])
-            if dist <= max_dist and sm_ini[j] > 0:
-                sm_i = np.append(sm_i, sm_ini[j])
-        if len(sm_i) >= min_neighbours:
-            sm_result[i] = np.average(sm_i)
-        else:
-            sm_result[i] = sm_ini[i]
-    return sm_result
-
 
 def storage(sm,T=1,Z_surface=150,Z_subsurface=1000):
     """Exponential filter to estimate soil moisture in the rootzone from surface observtions.
 
     Args:
         sm (list or array): Soil moisture in mm of water.
         T (float): Characteristic time length in the same units as the measurement interval.
@@ -963,15 +945,15 @@
     print('')
     print(f"Your cutoff rigidity is {Rc} GV")
     print(result)
     return result
 
 
 def estimate_lattice_water(clay_content, total_carbon=None):
-    """Estimate the amount of water in the lattice of clay minerals.
+    r"""Estimate the amount of water in the lattice of clay minerals.
 
     ![img1](img/lattice_water_simple.png) | ![img2](img/lattice_water_multiple.png)
     :-------------------------:|:-------------------------:
     $\omega_{lat} = 1.241 + 0.069 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
     Linear regression [lattice water (%) as a function of clay (%)] done with data from Soil Water Processes Lab and Dong and Ochsner (2018) |  Multiple linear regression [lattice water (%) as a function of clay (%) and soil carbon (%)] done with data from Soil Water Processes Lab.
 
     Args:
@@ -991,7 +973,263 @@
     if total_carbon is None:
         lattice_water = 1.241 + 0.069 * clay_content
     else:
         lattice_water = -0.028 + 0.077 * clay_content + 0.459 * total_carbon
     return lattice_water
 
 
+def latlon_to_utm(lat, lon, utm_zone_number, missing_values=None):
+    """Convert geographic coordinates (lat, lon) to projected coordinates (utm) using the Military Grid Reference System.
+
+    Function only applies to non-polar coordinates.
+    If further functionality is required, consider using the utm module. See references for more information.
+
+    ![UTM zones](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Universal_Transverse_Mercator_zones.svg/1920px-Universal_Transverse_Mercator_zones.svg.png)
+    UTM zones on an equirectangular world map with irregular zones in red and New York City's zone highlighted. See [UTM zones](https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system#UTM_zones) for a full description.
+
+
+    Args:
+        lat (float, array): Latitude in decimal degrees.
+        lon (float, array): Longitude in decimal degrees.
+        utm_zone_number (int): Universal Transverse Mercator (UTM) zone.
+
+    Returns:
+        (float, float): Tuple of easting and northing coordinates in meters. First element is easting, second is northing.
+
+    References:
+         Code adapted from utm module created by Tobias Bieniek (Github username: Turbo87)
+         [https://github.com/Turbo87/utm](https://github.com/Turbo87/utm)
+
+         [https://www.maptools.com/tutorials/grid_zone_details#](https://www.maptools.com/tutorials/grid_zone_details#)
+    """
+
+
+    # Define constants
+    R = 6_378_137  # Earth's radius at the Equator in meters
+
+    # Convert input data to Numpy arrays
+    if (type(lat) is not np.ndarray) or (type(lon) is not np.ndarray):
+        try:
+            lat = np.array(lat)
+            lon = np.array(lon)
+        except:
+            raise "Input values cannot be converted to Numpy arrays."
+
+    # Check latitude range
+    if np.any(lat < -80) | np.any(lat > 84):
+        raise "One or more latitude values exceed the range -80 to 84"
+
+    # Check longitude range
+    if np.any(lon < -180) | np.any(lon > 180):
+        raise "One or more longitude values exceed the range -180 to 180"
+
+    # Constants
+    K0 = 0.9996
+    E = 0.00669438
+    E_P2 = E / (1 - E)
+
+    M1 = (1 - E / 4 - 3 * E ** 2 / 64 - 5 * E ** 3 / 256)
+    M2 = (3 * E / 8 + 3 * E ** 2 / 32 + 45 * E ** 3 / 1024)
+    M3 = (15 * E ** 2 / 256 + 45 * E ** 3 / 1024)
+    M4 = (35 * E ** 3 / 3072)
+
+    # Trigonometric operations
+    lat_rad = np.radians(lat)
+    lon_rad = np.radians(lon)
+
+    lat_sin = np.sin(lat_rad)
+    lat_cos = np.cos(lat_rad)
+    lat_tan = lat_sin / lat_cos
+    lat_tan2 = lat_tan * lat_tan
+    lat_tan4 = lat_tan2 * lat_tan2
+
+    # Find central meridian.
+    central_lon = (utm_zone_number * 6 - 180) - 3  # Zones are every 6 degrees.
+    central_lon_rad = np.radians(central_lon)
+
+    n = R / np.sqrt(1 - E * lat_sin ** 2)
+    c = E_P2 * lat_cos ** 2
+
+    with np.errstate(divide='ignore', invalid='ignore'):
+        a = lat_cos * (np.remainder(((lon_rad - central_lon_rad) + np.pi), (2 * np.pi)) - np.pi)
+    m = R * (M1 * lat_rad - M2 * np.sin(2 * lat_rad) + M3 * np.sin(4 * lat_rad) - M4 * np.sin(6 * lat_rad))
+
+    easting = K0 * n * (a + a ** 3 / 6 * (1 - lat_tan2 + c) + a ** 5 / 120 * (
+                5 - 18 * lat_tan2 + lat_tan4 + 72 * c - 58 * E_P2)) + 500_000
+    northing = K0 * (m + n * lat_tan * (
+                a ** 2 / 2 + a ** 4 / 24 * (5 - lat_tan2 + 9 * c + 4 * c ** 2) + a ** 6 / 720 * (
+                    61 - 58 * lat_tan2 + lat_tan4 + 600 * c - 330 * E_P2)))
+
+    if np.any(lat < 0):
+        northing += 10_000_000
+
+    return easting, northing
+
+def euclidean_distance(px, py, x, y):
+    """Function that computes the Euclidean distance between one point
+    in space and one or more points.
+
+    Args:
+        px (float): x projected coordinate of the point.
+        py (float): y projected coordinate of the point.
+        x (list, ndarray, pandas.series): vector of x projected coordinates.
+        y (list, ndarray, pandas.series): vector of y projected coordinates.
+
+    Returns:
+        (ndarray): Numpy array of distances from the point (px,py) to all the points in x and y vectors.
+    """
+    d = np.sqrt((px - x) ** 2 + (py - y) ** 2)
+    return d
+
+
+def smooth_2D(x, y, z, buffer=100, min_neighbours=3, method='mean', rnd=False):
+    """Moving buffer filter to smooth georeferenced two-dimensional data.
+
+    Args:
+        x (list or array): UTM x coordinates in meters.
+        y (list or array): UTM y coordinates in meters.
+        z (list or array): Values to be smoothed.
+        buffer (float): Radial buffer distance in meters.
+        min_neighbours (int): Minimum number of neighbours to consider for the smoothing.
+        method (str): One of 'mean' or 'median'.
+        rnd (bool): Boolean to round the final result. Useful in case of z representing neutron counts.
+
+    Returns:
+        (array): Smoothed version of z with the same dimension as z.
+    """
+
+    # Convert input data to Numpy arrays
+    if (type(x) is not np.ndarray) or (type(y) is not np.ndarray):
+        try:
+            x = np.array(x)
+            y = np.array(y)
+        except:
+            raise "Input values cannot be converted to Numpy arrays."
+
+    if len(x) != len(y):
+        raise f"The number of x and y must be equal. Input x has {len(x)} values and y has {len(y)} values."
+
+    # Compute distances
+    N = len(x)
+    z_smooth = np.array([])
+    for k in range(N):
+        px = x[k]
+        py = y[k]
+
+        distances = euclidean_distance(px, py, x, y)
+        idx_within_buffer = distances <= buffer
+
+
+        if np.isnan(z[k]):
+            z_new_val = np.nan
+        elif len(distances[idx_within_buffer]) > min_neighbours:
+            if method == 'mean':
+                z_new_val = np.nanmean(z[idx_within_buffer])
+            elif method == 'median':
+                z_new_val = np.nanmedian(z[idx_within_buffer])
+            else:
+                raise f"Method {method} does not exist. Provide either 'mean' or 'median'."
+        else:
+            z_new_val = z[k] # If there are not enough neighbours, keep the original value
+
+        # Append smoothed value to array
+        z_smooth = np.append(z_smooth, z_new_val)
+
+    if rnd:
+        z_smooth = np.round(z_smooth, 0)
+
+    return z_smooth
+
+
+def idw(x, y, z, X_pred, Y_pred, neighborhood=1000, p=1):
+    """Function to interpolate data using inverse distance weight.
+
+    Args:
+        x (list or array): UTM x coordinates in meters.
+        y (list or array): UTM y coordinates in meters.
+        z (list or array): Values to be interpolated.
+        X_pred (list or array): UTM x coordinates where z values need to be predicted.
+        Y_pred (list or array): UTM y coordinates where z values need to be predicted.
+        neighborhood (float): Only points within this radius in meters are considered for the interpolation.
+        p (int): Exponent of the inverse distance weight formula. Typically, p=1 or p=2.
+
+    Returns:
+        (array): Interpolated values.
+
+    References:
+        [https://soilwater.github.io/pynotes-agriscience/notebooks/inverse_distance_weighting.html](https://soilwater.github.io/pynotes-agriscience/notebooks/inverse_distance_weighting.html)
+
+
+    """
+
+    # Flatten arrays to handle 1D and 2D arrays with the same code
+    s = X_pred.shape  # Save shape
+    X_pred = X_pred.flatten()
+    Y_pred = Y_pred.flatten()
+
+    # Pre-allocate output array
+    Z_pred = np.full_like(X_pred, np.nan)
+
+    for n in range(X_pred.size):
+        # Distance between current and observed points
+        d = euclidean_distance(X_pred[n], Y_pred[n], x, y)
+
+        # Select points within neighborhood only for interpolateion
+        idx_neighbors = d < neighborhood
+
+        # Compute interpolated value at point of interest
+        Z_pred[n] = np.sum(z[idx_neighbors] / d[idx_neighbors] ** p) / np.sum(1 / d[idx_neighbors] ** p)
+
+    return np.reshape(Z_pred, s)
+
+
+def interpolate_2D(x, y, z, dx=100, dy=100, method='cubic', neighborhood=1000):
+    """Function for interpolating irregular spatial data into a regular grid.
+
+    Args:
+        x (list or array): UTM x coordinates in meters.
+        y (list or array): UTM y coordinates in meters.
+        z (list or array): Values to be interpolated.
+        dx (float): Pixel width in meters.
+        dy (float): Pixel height in meters.
+        method (str): Interpolation method. One of 'cubic', 'linear', 'nearest', or 'idw'.
+        neighborhood (float): Only points within this radius in meters are considered for the interpolation.
+
+    Returns:
+        x_pred (array): 2D array with x coordinates.
+        y_pred (array): 2D array with y coordinates.
+        z_pred (array): 2D array with interpolated values.
+
+    References:
+        [https://soilwater.github.io/pynotes-agriscience/notebooks/interpolation.html](https://soilwater.github.io/pynotes-agriscience/notebooks/interpolation.html)
+    """
+
+    # Drop NaN values in x y and z
+    idx_nan = np.isnan(x) | np.isnan(y) | np.isnan(z)
+    x = x[~idx_nan]
+    y = y[~idx_nan]
+    z = z[~idx_nan]
+
+    if idx_nan.any():
+        print(f"WARNING: {np.isnan(x).sum()}, {np.isnan(y).sum()}, and {np.isnan(z).sum()} NaN values were dropped from x, y, and z.")
+
+    # Create 2D grid for interpolation
+    Nx = round((np.max(x) - np.min(x)) / dx) + 1
+    Ny = round((np.max(y) - np.min(y)) / dy) + 1
+    X_vec = np.linspace(np.min(x), np.max(x), Nx)
+    Y_vec = np.linspace(np.min(y), np.max(y), Ny)
+    X_pred, Y_pred = np.meshgrid(X_vec, Y_vec)
+
+    if method in ['linear', 'nearest', 'cubic']:
+        points = list(zip(x, y))
+        Z_pred = griddata(points, z, (X_pred, Y_pred), method=method)
+
+    elif method == 'idw':
+        Z_pred = idw(x, y, z, X_pred, Y_pred, neighborhood)
+
+    else:
+        raise f"Method {method} does not exist. Provide either 'cubic', 'linear', 'nearest', or 'idw'."
+
+    return X_pred, Y_pred, Z_pred
+
+
+
```

### Comparing `crnpy-0.2.post29/src/crnpy/data.py` & `crnpy-0.3.post1/src/crnpy/data.py`

 * *Files identical despite different names*

