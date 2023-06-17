# Comparing `tmp/finlogic-0.5.1.tar.gz` & `tmp/finlogic-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.5.1.tar", last modified: Mon May 29 09:58:56 2023, max compression
+gzip compressed data, was "finlogic-0.5.2.tar", last modified: Sat Jun 17 11:00:14 2023, max compression
```

## Comparing `finlogic-0.5.1.tar` & `finlogic-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.5.1/LICENSE
--rw-r--r--   0        0        0     9039 2023-05-26 08:29:09.365843 finlogic-0.5.1/README.md
--rw-r--r--   0        0        0      391 2023-05-29 09:45:14.175716 finlogic-0.5.1/finlogic/__init__.py
--rw-r--r--   0        0        0     5343 2023-05-29 09:53:24.121282 finlogic-0.5.1/finlogic/builder.py
--rw-r--r--   0        0        0    22909 2023-05-29 09:45:14.175716 finlogic-0.5.1/finlogic/company.py
--rw-r--r--   0        0        0      406 2023-05-27 17:07:48.111310 finlogic-0.5.1/finlogic/config.py
--rw-r--r--   0        0        0    10631 2023-05-29 09:45:14.175716 finlogic-0.5.1/finlogic/cvm.py
--rw-r--r--   0        0        0     5429 2023-05-27 17:20:46.327158 finlogic-0.5.1/finlogic/data_manager.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.5.1/finlogic/language.py
--rw-r--r--   0        0        0     1017 2023-05-29 09:58:56.796383 finlogic-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     3354 2023-05-25 23:18:10.569891 finlogic-0.5.1/tests/test_company.py
--rw-r--r--   0        0        0      907 2023-05-25 23:18:10.569891 finlogic-0.5.1/tests/test_data.py
--rw-r--r--   0        0        0    11118 1970-01-01 00:00:00.000000 finlogic-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.5.2/LICENSE
+-rw-r--r--   0        0        0     9039 2023-06-10 09:56:21.909374 finlogic-0.5.2/README.md
+-rw-r--r--   0        0        0      420 2023-06-17 10:42:32.134009 finlogic-0.5.2/finlogic/__init__.py
+-rw-r--r--   0        0        0    20572 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/company.py
+-rw-r--r--   0        0        0      718 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/config.py
+-rw-r--r--   0        0        0    10639 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/cvm.py
+-rw-r--r--   0        0        0     8060 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/data_manager.py
+-rw-r--r--   0        0        0     8463 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/indicators.py
+-rw-r--r--   0        0        0      708 2023-06-04 17:35:17.287141 finlogic-0.5.2/finlogic/language.py
+-rw-r--r--   0        0        0     6685 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/reports.py
+-rw-r--r--   0        0        0     1017 2023-06-17 11:00:14.741943 finlogic-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     3284 2023-06-08 13:02:11.720947 finlogic-0.5.2/tests/test_company.py
+-rw-r--r--   0        0        0      923 2023-06-17 10:40:57.986130 finlogic-0.5.2/tests/test_data.py
+-rw-r--r--   0        0        0    11118 1970-01-01 00:00:00.000000 finlogic-0.5.2/PKG-INFO
```

### Comparing `finlogic-0.5.1/LICENSE` & `finlogic-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.5.1/README.md` & `finlogic-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -164,16 +164,16 @@
 | net_income                   |     40.970 |      6.246 |    107.264 |
 | total_cash                   |     33.294 |     64.280 |     62.040 |
 | total_debt                   |    351.161 |    392.548 |    327.818 |
 | net_debt                     |    317.867 |    328.268 |    265.778 |
 | working_capital              |     -4.046 |      6.036 |     33.334 |
 | invested_capital             |    617.004 |    639.418 |    655.359 |
 | return_on_assets             |      0.062 |      0.035 |      0.140 |
-| return_on_capital            |      0.097 |      0.053 |      0.217 |
 | return_on_equity             |      0.144 |      0.020 |      0.344 |
+| roic                         |      0.097 |      0.053 |      0.217 |
 | gross_margin                 |      0.403 |      0.455 |      0.485 |
 | ebitda_margin                |      0.463 |      0.396 |      0.605 |
 | operating_margin             |      0.178 |      0.120 |      0.307 |
 | net_margin                   |      0.135 |      0.022 |      0.236 |
 
 ---
```

### Comparing `finlogic-0.5.1/finlogic/builder.py` & `finlogic-0.5.2/finlogic/reports.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,190 @@
 import pandas as pd
 from . import config as cfg
 
+SORT_COLS = [
+    "cvm_id",
+    "is_annual",
+    "is_consolidated",
+    "acc_code",
+    "period_reference",
+    "period_begin",
+    "period_end",
+]
+
 
 def read_all_processed_files() -> pd.DataFrame:
     """Read all processed CVM files."""
     # list filepaths in processed folder
     filepaths = sorted(cfg.CVM_PROCESSED_DIR.glob("*.pickle"))
     df = pd.concat([pd.read_pickle(f, compression="zstd") for f in filepaths])
-    return df
+    # df.query("cvm_id == 9512 and acc_code.isin(['1', '3.01'])", inplace=True)
+    # df.query("cvm_id == 9512", inplace=True)
+    return df.reset_index(drop=True)
 
 
 def drop_duplicated_entries(df: pd.DataFrame) -> pd.DataFrame:
     """Drop duplicated accounting entries before building database
 
     Because the report holds accounting entries for the year before, we can
     remove entries that are not most recent one. By doing this, we guarantee
     that there is only one valid accounting entry, the most recent one.
     """
-    sort_cols = [
-        "cvm_id",
-        "is_annual",
-        "is_consolidated",
-        "report_type",
-        "acc_code",
-        "period_reference",
-        "period_begin",
-        "period_end",
-    ]
-    df.sort_values(by=sort_cols, ascending=True, inplace=True, ignore_index=True)
-
-    subset_cols = sort_cols.copy()
+    df.sort_values(by=SORT_COLS, inplace=True, ignore_index=True)
+    subset_cols = SORT_COLS.copy()
     subset_cols.remove("period_reference")
+    df.drop_duplicates(subset=subset_cols, keep="last", ignore_index=True, inplace=True)
+
+    return df
+
+
+def insert_auxiliary_cols(df: pd.DataFrame):
+    """Insert aux. columns to help filter the dataframe."""
+    mask = ~df["is_annual"]
+    gr_last_quarter = df[mask].groupby(["cvm_id"])["period_end"].max()
+    df["last_quarter"] = df["cvm_id"].map(gr_last_quarter)
 
-    return df.drop_duplicates(subset=subset_cols, keep="last", ignore_index=True)
+    mask = df["is_annual"]
+    gr_last_annual = df[mask].groupby(["cvm_id"])["period_end"].max()
+    df["last_annual"] = df["cvm_id"].map(gr_last_annual)
+
+
+def drop_uncessary_quarters(df: pd.DataFrame) -> pd.DataFrame:
+    """Drop quarters that will not be used for building the reports and the
+    indicators dataframes."""
+
+    # Divide dataframe between annual and quarterly reports
+    dfa = df.query("is_annual").copy()
+    dfq = df.query("not is_annual").copy()
+
+    # The quarterly reports have two types of periods: accumulated and not
+    # accumulated. Only the accumulated periods will be used.
+    dfq.sort_values(by=SORT_COLS, inplace=True, ignore_index=True)
+    subset_cols = SORT_COLS.copy()
+    subset_cols.remove("period_begin")
+    dfq.drop_duplicates(
+        subset=subset_cols, keep="first", ignore_index=True, inplace=True
+    )
+
+    # Quarter mask
+    mask1 = dfq["last_quarter"] > dfq["last_annual"]
+    mask2 = dfq["period_end"] == dfq["last_quarter"]
+    mask3 = dfq["period_end"] == (dfq["last_quarter"] - pd.DateOffset(years=1))
+    mask = mask1 & (mask2 | mask3)
+
+    dfq = dfq.loc[mask].reset_index(drop=True)
+
+    return pd.concat([dfa, dfq], ignore_index=True)
+
+
+def get_ltm_mask(df: pd.DataFrame) -> pd.Series:
+    """Build a mask to divide the dataframe between data used in the LTM adjustment
+    and data that it not used in LTM adjustment.
+    The annual reports are not adjusted to LTM, only the quarterly reports are
+    adjusted. But we need to use the last annual report to adjust the quarterly
+    reports.
+    Conditions that need to be met for each company:
+        1  - Last quarter > last annual and
+        2a - Last "period_end" of annual reports or
+        2b - Last "period_reference" of quarterly reports and
+        3  - Only income, cash flow statements and EPS are adjusted to LTM
+    """
+    # Condition (1)
+    cond1 = df["last_quarter"] > df["last_annual"]
+
+    # Condition (2a)
+    mask1 = df["is_annual"]
+    mask2 = df["period_end"] == df["last_annual"]
+    cond2a = mask1 & mask2
+
+    # Condition (2b)
+    mask1 = ~df["is_annual"]
+    mask2 = df["period_reference"] == df["last_quarter"]
+    cond2b = mask1 & mask2
+
+    # Condition (3)
+    cond3 = df["acc_code"].str.startswith(("3", "6", "8"))
+
+    return cond1 & (cond2a | cond2b) & cond3
 
 
 def adjust_ltm(df: pd.DataFrame) -> pd.DataFrame:
     """Adjust income and cash flow statements to LTM (Last Twelve Months).
-    To get the LTM values, we     need to sum the current accumulated quarter
-    with the difference between the last annual value and the previous
-    accumulated quarter. Provided that quarterly values are always accumulated,
-    we can use the following formula:
-    LTM = current quarter + ( last annual - previous quarter)
+    To get the LTM values, we need to sum the current accumulated quarter with
+    the difference between the last annual value and the previous accumulated
+    quarter. Provided that quarterly values are always accumulated, we can use
+    the following formula:
+    LTM = current quarter + (last annual - previous quarter)
     Example for 1Q23: LTM = 1Q23 + (A22 - 1Q22)
     Example for 3Q23: LTM = 3Q23 + (A23 - 3Q23)
     """
-    # Quarters dataframe
-    quarters = df.query("not is_annual").reset_index(drop=True)
+    # Split dataframe between annual and quarterly reports
+    dfa = df.query("is_annual").copy()
+    dfq = df.query("not is_annual").reset_index(drop=True)
+
+    dfq["min_period_end"] = dfq.groupby("cvm_id")["period_end"].transform("min")
+    # Get prior quarter and invert the values
+    prior_quarter = dfq.query("period_end == min_period_end").copy()
+    prior_quarter["acc_value"] = -1 * prior_quarter["acc_value"]
 
-    # Get current quarter dataframe
-    grouped = quarters.groupby(["cvm_id", "is_consolidated", "acc_code"])["period_end"]
-    mask = quarters["period_end"] == grouped.transform("max")
-    current_quarter = quarters[mask].reset_index(drop=True)
-
-    # Get previous quarter dataframe
-    mask = quarters["period_end"] == grouped.transform("min")
-    previous_quarter = quarters[mask].reset_index(drop=True)
-    previous_quarter["acc_value"] = -previous_quarter["acc_value"]
-
-    # Annuals dataframe
-    annuals = df.query("is_annual").reset_index(drop=True)
-    # Last annual dataframe
-    grouped = annuals.groupby(["cvm_id", "is_consolidated", "acc_code"])["period_end"]
-    last_annual = annuals[annuals["period_end"] == grouped.transform("max")]
+    # Get current quarter
+    current_quarter = dfq.query("period_end == last_quarter").copy()
 
     # Build LTM adjusted dataframe
     ltm = (
-        pd.concat([current_quarter, previous_quarter, last_annual], ignore_index=True)[
+        pd.concat([current_quarter, dfa, prior_quarter])[
             ["cvm_id", "is_consolidated", "acc_code", "acc_value"]
         ]
         .groupby(by=["cvm_id", "is_consolidated", "acc_code"])
         .sum()
         .reset_index()
     )
-    # Use current_quarter as reference to insert the LTM values
-    current_quarter.drop(columns="acc_value", inplace=True)
-    ltm = pd.merge(current_quarter, ltm)
-    ltm["period_begin"] = quarters["period_end"] - pd.DateOffset(years=1)
-
-    return pd.concat([annuals, ltm], ignore_index=True)
 
+    # Current quarter receives LTM values
+    current_quarter.drop(columns=["acc_value"], inplace=True)
+    ltm = pd.merge(current_quarter, ltm)
+    ltm["period_begin"] = ltm["min_period_end"]
 
-def drop_not_last_quarter_end_period(df: pd.DataFrame) -> pd.DataFrame:
-    """Drop not last period end entries from df."""
-    # Separate the df in annual and quarterly
-    mask = df["is_annual"]
-    annual = df[mask].reset_index(drop=True)
-    quarterly = df[~mask].reset_index(drop=True)
+    # Prior quarter will not be used anymore
+    df = pd.concat([dfa, ltm], ignore_index=True)
 
-    # Remove not last period end entries from quarterly
-    grouped = quarterly.groupby(["cvm_id"])["period_end"]
-    mask = quarterly["period_end"] == grouped.transform("max")
-    adj_quarterly = quarterly[mask].reset_index(drop=True)
+    # Remove auxiliary columns
+    df.drop(columns=["min_period_end"], inplace=True)
 
-    # Concatenate the adjusted and non-adjusted dataframes
-    return pd.concat([annual, adj_quarterly], ignore_index=True)
+    return df
 
 
-def build_main_df():
-    """Build FinLogic Database from processed CVM files."""
+def save_reports():
+    """Save FinLogic Database from processed CVM files."""
     df = read_all_processed_files()
     df = drop_duplicated_entries(df)
+    insert_auxiliary_cols(df)
+    df = drop_uncessary_quarters(df)
 
-    # Divide the dataframe in what needs to be adjusted to LTM and what does not
-    # Only last "period_reference" entries are used in the LTM calculation
-    # Only income and cash flow statements are adjusted to LTM (report_type 3 and 6)
-    g_cols = ["cvm_id", "is_annual"]
-    df["max_period"] = df.groupby(g_cols)["period_reference"].transform("max")
-    mask1 = df["period_reference"] == df["max_period"]
-    mask2 = df["report_type"].isin([3, 6])
-    mask = mask1 & mask2
-    df.drop(columns=["max_period"], inplace=True)
-    ltm = df[mask].reset_index(drop=True)
-    not_ltm = df[~mask].reset_index(drop=True)
+    ltm_mask = get_ltm_mask(df)
+    # Separate the df in LTM and non-LTM
+    ltm = df[ltm_mask].reset_index(drop=True)
+    not_ltm = df[~ltm_mask].reset_index(drop=True)
 
     ltm = adjust_ltm(ltm)
 
     # Concatenate the adjusted and non-adjusted dataframes
     df = pd.concat([ltm, not_ltm], ignore_index=True)
 
-    # After the drop_unecessary entries, period_reference is not necessary anymore
-    # df.drop(columns=["period_reference"], inplace=True)
+    df.sort_values(by=SORT_COLS, ignore_index=True, inplace=True)
 
-    sort_cols = [
-        "cvm_id",
-        "is_annual",
-        "is_consolidated",
-        "report_type",
-        "acc_code",
-        "period_reference",
-        "period_begin",
-        "period_end",
-    ]
-    df.sort_values(by=sort_cols, ascending=True, inplace=True, ignore_index=True)
+    # Drop auxiliary columns
+    df.drop(columns=["last_quarter", "last_annual"], inplace=True)
 
     cat_cols = [c for c in df.columns if df[c].dtype in ["object"]]
     df[cat_cols] = df[cat_cols].astype("category")
 
-    df.to_pickle(cfg.DF_PATH, compression="zstd")
+    df.to_pickle(cfg.REPORTS_PATH, compression="zstd")
+
+
+def get_reports() -> pd.DataFrame:
+    """Return a DataFrame with all accounting data"""
+    if cfg.REPORTS_PATH.is_file():
+        df = pd.read_pickle(cfg.REPORTS_PATH, compression="zstd")
+    else:
+        df = pd.DataFrame()
+    return df
```

### Comparing `finlogic-0.5.1/finlogic/company.py` & `finlogic-0.5.2/finlogic/company.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     numexpr does not support extension array dtypes (category not supported
     yet). Please set your engine to python manually. That means that the query
     method has to use engine='python' to work with category dtype. N.B. Only
     FinLogic Dataframe uses category dtype for efficiency.
 
 """
 from typing import Literal
-import numpy as np
 import pandas as pd
 from .language import language_df
-from . import data_manager as dm
+from . import reports as rep
+from . import indicators as ind
 
 
 class Company:
     """A class to represent a company financial data.
 
      This class provides methods to create financial reports and to calculate
      financial indicators based on a company's accounting data. The class also
@@ -56,15 +56,15 @@
          ValueError: If the input arguments are invalid.
     """
 
     def __init__(
         self,
         identifier: int | str,
         is_consolidated: bool = True,
-        acc_unit: int | float | Literal["t", "m", "b"] = 1,
+        acc_unit: float | Literal["t", "m", "b"] = 1.0,
         tax_rate: float = 0.34,
         language: Literal["english", "portuguese"] = "english",
     ):
         """Initializes a new instance of the Company class."""
         self._initialized = False
         self.identifier = identifier
         self.is_consolidated = is_consolidated
@@ -98,15 +98,15 @@
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
         df = (
-            dm.get_main_df()[["cvm_id", "tax_id", "name_id"]]
+            rep.get_reports()[["cvm_id", "tax_id", "name_id"]]
             .query("cvm_id == @identifier or tax_id == @identifier")
             .drop_duplicates(ignore_index=True)
         )
         if not df.empty:
             self._cvm_id = df.loc[0, "cvm_id"]
             self.tax_id = df.loc[0, "tax_id"]
             self.name_id = df.loc[0, "name_id"]
@@ -126,15 +126,15 @@
         Consolidated accounting combines the financial statements of a parent
         company and its subsidiaries, while separate accounting keeps them
         separate. Defaults to 'consolidated'.
 
         Raises:
             ValueError: If the accounting method is invalid.
         """
-        return self._acc_unit
+        return self._is_consolidated
 
     @is_consolidated.setter
     def is_consolidated(self, value: bool):
         if type(value) is bool:
             self._is_consolidated = value
         else:
             raise ValueError("Company 'is_consolidated' value is invalid")
@@ -165,22 +165,22 @@
 
             To set the accounting unit to a custom factor, e.g., 10,000:
                 company.acc_unit = 10_000
         """
         return self._acc_unit
 
     @acc_unit.setter
-    def acc_unit(self, value: int | float | Literal["t", "m", "b"]):
+    def acc_unit(self, value: float | Literal["t", "m", "b"]):
         match value:
             case "t":
-                self._acc_unit = 1_000
+                self._acc_unit = 1_000.0
             case "m":
-                self._acc_unit = 1_000_000
+                self._acc_unit = 1_000_000.0
             case "b":
-                self._acc_unit = 1_000_000_000
+                self._acc_unit = 1_000_000_000.0
             case str():  # Add this case to catch invalid strings
                 raise ValueError("Invalid string for Accounting Unit")
             case v if v > 0:
                 self._acc_unit = float(v)
             case _:
                 raise ValueError("Accounting Unit is invalid")
 
@@ -249,39 +249,30 @@
     def _set_df(self) -> pd.DataFrame:
         """Sets the company data frame.
 
         This method creates a dataframe with the company's financial
         statements.
         """
         df = (
-            dm.get_main_df()
+            rep.get_reports()
             .query(
                 "cvm_id == @self._cvm_id and \
                  is_consolidated == @self._is_consolidated"
             )
             .reset_index(drop=True)
         )
 
         # Convert category columns back to string
         columns = df.columns
         cat_cols = [c for c in columns if df[c].dtype == "category"]
         df[cat_cols] = df[cat_cols].astype("string")
 
-        # Change acc_value only when it is not earnings_per_share (report_type 8)
-        df["acc_value"] = np.where(
-            df["report_type"] == 8,
-            df["acc_value"],
-            df["acc_value"] / self._acc_unit,
-        )
-
-        # Remove quarters entries that are not the last one
-        mask1 = ~df["is_annual"]
-        mask2 = df["period_end"] != df["period_end"].max()
-        mask = mask1 & mask2
-        df = df[~mask].reset_index(drop=True)
+        # Adjust for unit change only where it is not EPS (acc_code 8...)
+        mask = ~df["acc_code"].str.startswith("8")
+        df.loc[mask, "acc_value"] = df.loc[mask, "acc_value"] / self._acc_unit
 
         self._first_period = df["period_end"].min()
         self._last_period = df["period_end"].max()
 
         # Not necessarily there will be a quarterly report for the last period
         self._last_annual = df.query("is_annual")["period_end"].max()
 
@@ -299,14 +290,19 @@
         )
 
         # Set company data frame
         self._df = df
 
     def info(self) -> pd.DataFrame:
         """Print a concise summary of a company."""
+        if self._df.empty:
+            acc_method = "consolidated" if self._is_consolidated else "separate"
+            print("There is no avaible accounting data for:")
+            print(f"    cvm_id = {self._cvm_id} and accounting method = {acc_method}")
+            return None
         company_info = {
             "Name": self.name_id,
             "CVM ID": self._cvm_id,
             "Fiscal ID (CNPJ)": self.tax_id,
             "Total Accounting Rows": len(self._df.index),
             "Selected Accounting Method": "consolidated"
             if self._is_consolidated
@@ -317,15 +313,16 @@
             "Last Report": self._last_period.strftime("%Y-%m-%d"),
             "Last Report Type": self._last_period_type,
         }
         s = pd.Series(company_info)
         s.name = "Company Info"
         return s.to_frame()
 
-    def _build_report_index(self, dfi: pd.DataFrame) -> pd.DataFrame:
+    @staticmethod
+    def _build_report_index(dfi: pd.DataFrame) -> pd.DataFrame:
         """Build the index for the report. This function is used by the
         _build_report function. The index is built from the annual reports
         "acc_code" works as a primary key. Other columns set the preference order
         """
         df = (
             dfi[["acc_code", "acc_name", "period_end"]]
             .sort_values(by=["acc_code", "period_end"])
@@ -346,14 +343,34 @@
             if period == self._last_period and self._last_period_type == "quarterly":
                 period_str += " ltm"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
             dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
         dfo.fillna(0, inplace=True)
         return dfo.sort_values("acc_code", ignore_index=True)
 
+    @staticmethod
+    def _remove_not_last_quarters(df: pd.DataFrame) -> pd.DataFrame:
+        """Remove quarters that are not the last one.
+
+        This function removes quarters that are not the last one.
+        This is useful when generating reports.
+
+        Args:
+            df: Dataframe with the financial statements.
+
+        Returns:
+            Dataframe with the financial statements without the quarters that are not
+            the last one.
+        """
+        mask1 = ~df["is_annual"]
+        mask2 = df["period_end"] != df["period_end"].max()
+        mask = mask1 & mask2
+        df = df[~mask].reset_index(drop=True)
+        return df
+
     def report(
         self,
         report_type: Literal[
             "balance_sheet",
             "assets",
             "cash",
             "current_assets",
@@ -410,14 +427,15 @@
             pd.DataFrame: Generated financial report as a pandas DataFrame.
 
         Raises:
             ValueError: If some argument is invalid.
         """
         # Copy company dataframe to avoid changing it
         df = self._df.copy()
+        df = self._remove_not_last_quarters(df)
         # Check input arguments.
         if acc_level not in [0, 1, 2, 3, 4]:
             raise ValueError("acc_level expects 0, 1, 2, 3 or 4")
 
         # Filter dataframe for selected acc_level
         # Example of an acc_code: "7.08.04.04" -> 4 levels and 3 dots
         if acc_level:
@@ -432,15 +450,15 @@
 
         if self._language == "English":
             _pten_dict = dict(language_df.values)
             _pten_dict = MyDict(_pten_dict)
             df["acc_name"] = df["acc_name"].map(_pten_dict)
 
         """
-        Filter dataframe for selected report_type (report type)
+        Filter dataframe for selected acc_code
         df['acc_code'].str[0].unique() -> [1, 2, 3, 4, 5, 6, 7]
         The first part of 'acc_code' is the report type
         Table of reports correspondence:
             1 -> Balance Sheet - Assets
             2 -> Balance Sheet - Liabilities and Shareholders’ Equity
             3 -> Income
             4 -> Comprehensive Income
@@ -503,96 +521,27 @@
         df = (
             pd.concat([df_bs, df_is, df_cf])
             .query(f"acc_code == {acc_list}")
             .reset_index(drop=True)
         )
         return df
 
-    @staticmethod
-    def _prior_values(s: pd.Series, is_prior: bool) -> pd.Series:
-        """Shift row to the right in order to obtain series previous values"""
-        if is_prior:
-            arr = s.iloc[:-1].values
-            return np.append(np.nan, arr)
-        else:
-            return s
-
-    def indicators(self, num_years: int = 0, is_prior: bool = True) -> pd.DataFrame:
+    def indicators(self, num_years: int = 0) -> pd.DataFrame:
         """Calculate the company main operating indicators.
 
         Args:
             num_years: Number of years to consider for calculation. If 0, use
                 all available years. Defaults to 0.
-            is_prior: Divide return measurements by book values from the end of
-                the prior year (see Damodaran reference). Defaults to True.
 
         Returns:
             pd.DataFrame: Dataframe containing calculated financial indicators.
-
-        References:
-            [1] Aswath Damodaran, "Return on Capital (ROC), Return on Invested
-                Capital (ROIC) and Return on Equity (ROE): Measurement and
-                Implications.", 2007,
-                https://people.stern.nyu.edu/adamodar/pdfoles/papers/returnmeasures.pdf
-                https://people.stern.nyu.edu/adamodar/New_Home_Page/datafile/variable.htm
-        """
-        df_bs = self.report("balance_sheet")
-        df_is = self.report("income_statement")
-        df_cf = self.report("cash_flow")
-        df = (
-            pd.concat([df_bs, df_is, df_cf])
-            .drop(columns=["acc_name"])
-            .set_index("acc_code", drop=True)
-        )
-
-        # Calculate indicators series
-        revenues = df.loc["3.01"]
-        gross_profit = df.loc["3.03"]
-        ebit = df.loc["3.05"]
-        ebt = df.loc["3.07"]
-        effective_tax = df.loc["3.08"]
-        depreciation_amortization = df.loc["6.01.01.04"]
-        ebitda = ebit + depreciation_amortization
-        operating_cash_flow = df.loc["6.01"]
-        # capex = df.loc["6.02"]
-        net_income = df.loc["3.11"]
-        total_assets = df.loc["1"]
-        total_assets_p = self._prior_values(total_assets, is_prior)
-        equity = df.loc["2.03"]
-        equity_p = self._prior_values(equity, is_prior)
-        total_cash = df.loc["1.01.01"] + df.loc["1.01.02"]
-        current_assets = df.loc["1.01"]
-        current_liabilities = df.loc["2.01"]
-        working_capital = current_assets - current_liabilities
-        total_debt = df.loc["2.01.04"] + df.loc["2.02.01"]
-        net_debt = total_debt - total_cash
-        invested_capital = total_debt + equity - total_cash
-        invested_capital_p = self._prior_values(invested_capital, is_prior)
-
-        # Output Dataframe (dfo)
-        dfo = pd.DataFrame(columns=df.columns)
-        dfo.loc["revenues"] = revenues
-        dfo.loc["operating_cash_flow"] = operating_cash_flow
-        # dfo.loc["capex"] = capex
-        dfo.loc["ebitda"] = ebitda
-        dfo.loc["ebit"] = ebit
-        dfo.loc["ebt"] = ebt
-        dfo.loc["effective_tax_rate"] = -1 * effective_tax / ebt
-        dfo.loc["net_income"] = net_income
-        dfo.loc["total_cash"] = total_cash
-        dfo.loc["total_debt"] = total_debt
-        dfo.loc["net_debt"] = net_debt
-        dfo.loc["working_capital"] = working_capital
-        dfo.loc["invested_capital"] = invested_capital
-        dfo.loc["return_on_assets"] = ebit * (1 - self._tax_rate) / total_assets_p
-        dfo.loc["return_on_capital"] = ebit * (1 - self._tax_rate) / invested_capital_p
-        dfo.loc["return_on_equity"] = net_income / equity_p
-        dfo.loc["gross_margin"] = gross_profit / revenues
-        dfo.loc["ebitda_margin"] = ebitda / revenues
-        dfo.loc["pre_tax_operating_margin"] = ebit / revenues
-        dfo.loc["after_tax_operating_margin"] = ebit * (1 - self._tax_rate) / revenues
-        dfo.loc["net_margin"] = net_income / revenues
-
+        """
+        expr = "cvm_id == @self._cvm_id and is_consolidated == @self._is_consolidated"
+        dfi = ind.get_indicators().query(expr)
+        dfo = ind.format_indicators(dfi, unit=self._acc_unit)
+        # Columns cvm_id and is_consolidated are redundant for the Company class
+        dfo.drop(columns=["cvm_id", "is_consolidated"], inplace=True)
         # Show only the selected number of years
         if num_years > 0:
-            dfo = dfo[dfo.columns[-num_years:]]
+            dfo = dfo[dfo.columns[-num_years:]].copy()
+
         return dfo
```

### Comparing `finlogic-0.5.1/finlogic/cvm.py` & `finlogic-0.5.2/finlogic/cvm.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,27 +74,29 @@
         # print(f"    {CHECKMARK} {filename} updated.")
         if filepath:
             updated_filepaths.append(filepath)
     s.close()
     return updated_filepaths
 
 
-def read_raw_file(filepath: Path) -> pd.DataFrame:
+def read_raw_file(filepath: Path, companies_to_process: List[int]) -> pd.DataFrame:
     """Read annual file, process it, save the result and return the file path."""
     cvm_zipfile = zf.ZipFile(filepath)
     child_filenames = cvm_zipfile.namelist()
 
     # Filename example for the first file in zip: "dfp_cia_aberta_2022.csv"
     # Do not read the first file, since it is a metadata file.
     child_filenames = child_filenames[1:]
 
     df_list = []
     for child_filename in child_filenames:
         child_zf = cvm_zipfile.open(child_filename)
         child_df = pd.read_csv(child_zf, sep=";", encoding="iso-8859-1")
+        if companies_to_process:
+            child_df.query("CD_CVM in @companies_to_process", inplace=True)
         df_list.append(child_df)
     df = pd.concat(df_list, ignore_index=True)
     return df
 
 
 def remove_empty_spaces(s: pd.Series) -> pd.Series:
     """Remove empty spaces in a pandas Series of repeated strings."""
@@ -229,44 +231,41 @@
     """
     map_dic = {"Con": True, "Ind": False}
     df.insert(4, "is_consolidated", df["report_group"].str[3:6].map(map_dic))
 
     # 'report_group' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
 
-    # "report_type" will be used to fast filter the data. Otherwise, it would be
-    # necessary to use str.startswith() or str.contains() methods.
-    df.insert(5, "report_type", df["acc_code"].str[0])
-    df["report_type"] = df["report_type"].astype("uint8")
-
     # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
     # Few of them have different values in "acc_value". Only one them will be kept.
     # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
     cols.remove("acc_value")
     df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
 
     return df
 
 
-def process_file(raw_filepath: Path) -> Path:
+def process_file(raw_filepath: Path, companies_to_process: List[int]) -> Path:
     """Read, process and save a CVM file."""
-    df = read_raw_file(raw_filepath)
+    df = read_raw_file(raw_filepath, companies_to_process)
     df = process_df(df, raw_filepath)
     processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".pickle")
     # save_processed_df(df, processed_filepath)
     df.to_pickle(processed_filepath, compression="zstd")
     return processed_filepath
 
 
-def process_files_with_progress(filepaths_to_process):
+def process_files_with_progress(
+    filepaths_to_process: List[Path], companies_to_process: List[int]
+):
     """Process CVM files with a progress bar."""
     for filepath in tqdm(filepaths_to_process, desc="Processing..."):
         # print(f"    {CHECKMARK} {raw_filepath.name} processed.")
-        process_file(filepath)
+        process_file(filepath, companies_to_process)
 
 
 def get_raw_file_mtimes() -> pd.DataFrame:
     """Return a Pandas DataFrame with file_source and file_mtime columns."""
     filepaths = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
     d_mtimes = {filepath.name: filepath.stat().st_mtime for filepath in filepaths}
     return pd.DataFrame(d_mtimes.items(), columns=["file_source", "file_mtime"])
```

### Comparing `finlogic-0.5.1/finlogic/language.py` & `finlogic-0.5.2/finlogic/language.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from pathlib import Path
 import pandas as pd
 from . import config as cfg
 
 INTERIM_DIR = cfg.DATA_PATH / "interim"
-LANGUAGE_DF_PATH = INTERIM_DIR / "pten_df.csv"
+LANGUAGE_REPORTS_PATH = INTERIM_DIR / "pten_df.csv"
 URL_LANGUAGE = "https://raw.githubusercontent.com/fe-lipe-c/finlogic_datasets/master/data/pten_df.csv"  # noqa
 
 # Create interim folder if it does not exist.
 Path.mkdir(INTERIM_DIR, parents=True, exist_ok=True)
 
 # Start/load language file data
-if LANGUAGE_DF_PATH.is_file():
-    language_df = pd.read_csv(LANGUAGE_DF_PATH)
+if LANGUAGE_REPORTS_PATH.is_file():
+    language_df = pd.read_csv(LANGUAGE_REPORTS_PATH)
 else:
     language_df = pd.DataFrame()
 
 
 def process_language_df():
     """Process language dataframe."""
     language_df = pd.read_csv(URL_LANGUAGE)
-    language_df.to_csv(LANGUAGE_DF_PATH, index=False)
+    language_df.to_csv(LANGUAGE_REPORTS_PATH, index=False)
```

### Comparing `finlogic-0.5.1/pyproject.toml` & `finlogic-0.5.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 dependencies = [
     "pandas>=1.5.0",
     "requests>=2.30.0",
     "tqdm>=4.1.0",
     "zstandard>=0.21.0",
 ]
-version = "0.5.1"
+version = "0.5.2"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.5.1/tests/test_company.py` & `finlogic-0.5.2/tests/test_company.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,30 +51,26 @@
         petro_indicators_sep = self.petro_sep.indicators()
         petro_indicators_con = self.petro_con.indicators()
         # Get the indicators (rounded to 4 decimals)
         revenues_2009_sep = round(petro_indicators_sep.at["revenues", "2009-12-31"], 4)
         total_debt_2015_sep = round(
             petro_indicators_sep.at["total_debt", "2015-12-31"], 4
         )
-        roic_2021_sep = round(
-            petro_indicators_sep.at["return_on_capital", "2021-12-31"], 4
-        )
+        roic_2021_sep = round(petro_indicators_sep.at["roic", "2021-12-31"], 4)
         # Get the indicators (rounded to 4 decimals)
         revenues_2009_con = round(petro_indicators_con.at["revenues", "2009-12-31"], 4)
         total_debt_2015_con = round(
             petro_indicators_con.at["total_debt", "2015-12-31"], 4
         )
-        roic_2021_con = round(
-            petro_indicators_con.at["return_on_capital", "2021-12-31"], 4
-        )
+        roic_2021_con = round(petro_indicators_con.at["roic", "2021-12-31"], 4)
         # Check the indicators
-        self.assertEqual(roic_2021_sep, 0.1623)
+        self.assertEqual(roic_2021_sep, 0.1512)
         self.assertEqual(revenues_2009_sep, 134.0339)
         self.assertEqual(total_debt_2015_sep, 305.3460)
         # Check the indicators
-        self.assertEqual(roic_2021_con, 0.2176)
+        self.assertEqual(roic_2021_con, 0.2149)
         self.assertEqual(revenues_2009_con, 182.8338)
         self.assertEqual(total_debt_2015_con, 493.0230)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `finlogic-0.5.1/tests/test_data.py` & `finlogic-0.5.2/tests/test_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import unittest
+from datetime import datetime
 import finlogic as fl
 from finlogic import data_manager as dm
 
 
 class TestData(unittest.TestCase):
     def test_info(self):
         """Test the info method of the Database module."""
         info = dm.info()["FinLogic Info"]
-        self.assertEqual(info["first_report"], "2009-01-31")
-        self.assertTrue(info["accounting_entries"] > 2_000_000)
+        first_report = datetime.strptime(info["first_report"], "%Y-%m-%d")
+        self.assertTrue(first_report.year <= 2009)
+        self.assertTrue(info["accounting_entries"] > 1_000_000)
 
     def test_search_company(self):
         """Test the search_company method of the Database module."""
-        search_result = fl.search_company("petrobras")
+        search_result = fl.search_company("3r")
         """
-            name_id                            cvm_id  tax_id
-        0   PETROBRAS DISTRIBUIDORA S/A         24295  34.274.233/0001-02
-        1   PETROLEO BRASILEIRO S.A. PETROBRAS   9512  33.000.167/0001-01
+            name_id cvm_id  tax_id  segment is_restructuring    most_traded_stock
+        0	3R ...  25291   12...   expl... False	            RRRP3
         """
-        # Check the results
-        self.assertEqual(set(search_result["cvm_id"]), {9512, 24295})
+        # Check results
+        self.assertEqual(set(search_result["cvm_id"]), {25291})
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `finlogic-0.5.1/PKG-INFO` & `finlogic-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.5.1
+Version: 0.5.2
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -207,16 +207,16 @@
 | net_income                   |     40.970 |      6.246 |    107.264 |
 | total_cash                   |     33.294 |     64.280 |     62.040 |
 | total_debt                   |    351.161 |    392.548 |    327.818 |
 | net_debt                     |    317.867 |    328.268 |    265.778 |
 | working_capital              |     -4.046 |      6.036 |     33.334 |
 | invested_capital             |    617.004 |    639.418 |    655.359 |
 | return_on_assets             |      0.062 |      0.035 |      0.140 |
-| return_on_capital            |      0.097 |      0.053 |      0.217 |
 | return_on_equity             |      0.144 |      0.020 |      0.344 |
+| roic                         |      0.097 |      0.053 |      0.217 |
 | gross_margin                 |      0.403 |      0.455 |      0.485 |
 | ebitda_margin                |      0.463 |      0.396 |      0.605 |
 | operating_margin             |      0.178 |      0.120 |      0.307 |
 | net_margin                   |      0.135 |      0.022 |      0.236 |
 
 ---
```

