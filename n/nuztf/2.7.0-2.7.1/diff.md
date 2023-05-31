# Comparing `tmp/nuztf-2.7.0.tar.gz` & `tmp/nuztf-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuztf-2.7.0.tar", max compression
+gzip compressed data, was "nuztf-2.7.1.tar", max compression
```

## Comparing `nuztf-2.7.0.tar` & `nuztf-2.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-22 11:02:48.219604 nuztf-2.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2812 2023-05-22 11:02:48.219604 nuztf-2.7.0/README.md
--rw-r--r--   0        0        0     5496 2023-05-22 11:02:48.239604 nuztf-2.7.0/nuztf/TNS_submit.py
--rw-r--r--   0        0        0      123 2023-05-22 11:02:48.239604 nuztf-2.7.0/nuztf/__init__.py
--rw-r--r--   0        0        0    19445 2023-05-22 11:02:48.239604 nuztf-2.7.0/nuztf/ampel_api.py
--rw-r--r--   0        0        0    48216 2023-05-22 11:02:48.239604 nuztf-2.7.0/nuztf/base_scanner.py
--rw-r--r--   0        0        0     8356 2023-05-22 11:02:48.239604 nuztf-2.7.0/nuztf/cat_match.py
--rw-r--r--   0        0        0      442 2023-05-22 11:02:48.239604 nuztf-2.7.0/nuztf/config/gw_run_config.yaml
--rw-r--r--   0        0        0      438 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/config/nu_run_config.yaml
--rw-r--r--   0        0        0     2864 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/credentials.py
--rw-r--r--   0        0        0     3222 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/flatpix.py
--rw-r--r--   0        0        0     1354 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/fritz.py
--rw-r--r--   0        0        0    15370 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/irsa.py
--rw-r--r--   0        0        0     7692 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/neutrino_scanner.py
--rw-r--r--   0        0        0     9788 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/observations.py
--rw-r--r--   0        0        0     4529 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/observations_depot.py
--rw-r--r--   0        0        0     6608 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/parse_nu_gcn.py
--rw-r--r--   0        0        0      902 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/paths.py
--rw-r--r--   0        0        0    11585 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/plot.py
--rw-r--r--   0        0        0    13181 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/skymap.py
--rw-r--r--   0        0        0    16196 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/skymap_scanner.py
--rw-r--r--   0        0        0     1051 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/style.py
--rw-r--r--   0        0        0     5241 2023-05-22 11:02:48.243604 nuztf-2.7.0/nuztf/utils.py
--rw-r--r--   0        0        0     1760 2023-05-22 11:02:48.247604 nuztf-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     5021 1970-01-01 00:00:00.000000 nuztf-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 13:00:18.695730 nuztf-2.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     2812 2023-05-31 13:00:18.695730 nuztf-2.7.1/README.md
+-rw-r--r--   0        0        0     5496 2023-05-31 13:00:18.715730 nuztf-2.7.1/nuztf/TNS_submit.py
+-rw-r--r--   0        0        0      123 2023-05-31 13:00:18.715730 nuztf-2.7.1/nuztf/__init__.py
+-rw-r--r--   0        0        0    19445 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/ampel_api.py
+-rw-r--r--   0        0        0    48570 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/base_scanner.py
+-rw-r--r--   0        0        0     8356 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/cat_match.py
+-rw-r--r--   0        0        0      442 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/config/gw_run_config.yaml
+-rw-r--r--   0        0        0      438 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/config/nu_run_config.yaml
+-rw-r--r--   0        0        0     2864 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/credentials.py
+-rw-r--r--   0        0        0     3222 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/flatpix.py
+-rw-r--r--   0        0        0     1354 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/fritz.py
+-rw-r--r--   0        0        0    15370 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/irsa.py
+-rw-r--r--   0        0        0     7692 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/neutrino_scanner.py
+-rw-r--r--   0        0        0     9788 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/observations.py
+-rw-r--r--   0        0        0     4529 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/observations_depot.py
+-rw-r--r--   0        0        0     6608 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/parse_nu_gcn.py
+-rw-r--r--   0        0        0      902 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/paths.py
+-rw-r--r--   0        0        0    11585 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/plot.py
+-rw-r--r--   0        0        0    13356 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/skymap.py
+-rw-r--r--   0        0        0    16196 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/skymap_scanner.py
+-rw-r--r--   0        0        0     1051 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/style.py
+-rw-r--r--   0        0        0     5241 2023-05-31 13:00:18.719730 nuztf-2.7.1/nuztf/utils.py
+-rw-r--r--   0        0        0     1760 2023-05-31 13:00:18.723730 nuztf-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5021 1970-01-01 00:00:00.000000 nuztf-2.7.1/PKG-INFO
```

### Comparing `nuztf-2.7.0/LICENSE.txt` & `nuztf-2.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/README.md` & `nuztf-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/TNS_submit.py` & `nuztf-2.7.1/nuztf/TNS_submit.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/ampel_api.py` & `nuztf-2.7.1/nuztf/ampel_api.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/base_scanner.py` & `nuztf-2.7.1/nuztf/base_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pathlib import Path
 
 import backoff
 import healpy as hp
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas
 import pandas as pd
 import requests
 from ampel.ztf.alert.ZiAlertSupplier import ZiAlertSupplier
 from ampel.ztf.dev.DevAlertConsumer import DevAlertConsumer
 from ampel.ztf.t0.DecentFilter import DecentFilter
 from astropy import units as u
 from astropy.coordinates import Distance, SkyCoord
@@ -216,14 +215,15 @@
             self.add_res_to_cache(query_res)
 
     def check_ampel_filter(self, ztf_name):
         lvl = logging.getLogger().getEffectiveLevel()
         logging.getLogger().setLevel(logging.DEBUG)
         self.logger.info("Set logger level to DEBUG")
         all_query_res = ampel_api_name(ztf_name, logger=self.logger)
+        assert len(all_query_res) > 0, f"No results from ampel api for {ztf_name}"
         pipeline_bool = False
         for query_res in all_query_res:
             self.logger.info("Checking filter f (no prv)")
             no_prv_bool = self.filter_f_no_prv(query_res)
             self.logger.info(f"Filter f (np prv): {no_prv_bool}")
             if no_prv_bool:
                 self.logger.info("Checking ampel filter")
@@ -544,20 +544,20 @@
 
         :return None:
         """
         if len(self.cache.items()) == 0:
             self.logger.info("No candidates found, skipping pdf creation")
             return
 
-        pdf_path = self.get_output_dir().joinpath("candidates.pdf")
+        pdf_path = self.get_output_dir() / "candidates.pdf"
 
         self.logger.info(
-            f"Creating overview pdf at: {pdf_path}\n"
-            f"(this might take a moment as it involves catalog matching)"
+            f"Creating overview pdf\n(this might take a moment as it involves catalog matching)"
         )
+        self.logger.debug(f"Overview pdf path: {pdf_path}")
 
         with PdfPages(pdf_path) as pdf:
             for name, alert in tqdm(sorted(self.cache.items())):
                 fig, _ = lightcurve_from_alert(
                     [alert],
                     include_cutouts=True,
                     logger=self.logger,
@@ -573,17 +573,18 @@
 
         :return None:
         """
         if len(self.cache.items()) == 0:
             self.logger.info("No candidates found, skipping csv creation")
             return
 
-        csv_path = self.get_output_dir().joinpath("candidate_table.csv")
+        csv_path = self.get_output_dir() / "candidate_table.csv"
 
-        self.logger.info(f"Creating overview csv at {csv_path}")
+        self.logger.info("Creating overview csv")
+        self.logger.debug(f"Overview csv path: {csv_path}")
 
         data = {
             "ztf_id": [],
             "RA": [],
             "Dec": [],
             "mag": [],
             "xmatch": [],
@@ -597,15 +598,15 @@
             data["mag"].append(alert["candidate"]["magpsf"])
             data["xmatch"].append(get_cross_match_info(raw=alert, logger=self.logger))
             if alert.get("kilonova_eval") is not None:
                 data["kilonova_score"].append(alert["kilonova_eval"]["kilonovaness"])
             else:
                 data["kilonova_score"].append(None)
 
-        df = pandas.DataFrame.from_dict(data)
+        df = pd.DataFrame.from_dict(data)
 
         df.to_csv(csv_path)
 
     def tns_summary(self):
         """
         Create summary for TNS
 
@@ -1028,40 +1029,46 @@
         )
 
         self.logger.info("Unpacking observations")
 
         pix_map = dict()
         pix_obs_times = dict()
 
-        # field_pix = get_flatpix(nside=self.nside, logger=self.logger)
         nested_pix = get_nested_pix(nside=self.nside, logger=self.logger)
 
         for i, obs_time in enumerate(tqdm(list(set(data["obsjd"])))):
             obs = data[data["obsjd"] == obs_time]
 
             field = obs["field_id"].iloc[0]
 
-            flat_pix = nested_pix[field]
-
-            mask = obs["status"] == 0
-            indices = obs["qid"].values[mask]
+            try:
+                flat_pix = nested_pix[field]
 
-            for qid in indices:
-                pixels = flat_pix[qid]
+                mask = obs["status"] == 0
+                indices = obs["qid"].values[mask]
 
-                for p in pixels:
-                    if p not in pix_obs_times.keys():
-                        pix_obs_times[p] = [obs_time]
-                    else:
-                        pix_obs_times[p] += [obs_time]
+                for qid in indices:
+                    pixels = flat_pix[qid]
 
-                    if p not in pix_map.keys():
-                        pix_map[p] = [field]
-                    else:
-                        pix_map[p] += [field]
+                    for p in pixels:
+                        if p not in pix_obs_times.keys():
+                            pix_obs_times[p] = [obs_time]
+                        else:
+                            pix_obs_times[p] += [obs_time]
+
+                        if p not in pix_map.keys():
+                            pix_map[p] = [field]
+                        else:
+                            pix_map[p] += [field]
+
+            except KeyError:
+                self.logger.warning(
+                    f"Field {field} not found in nested pix dict. "
+                    f"This might be an engineering observation."
+                )
 
         npix = hp.nside2npix(self.nside)
         theta, phi = hp.pix2ang(self.nside, np.arange(npix), nest=False)
         radecs = SkyCoord(ra=phi * u.rad, dec=(0.5 * np.pi - theta) * u.rad)
         idx = np.where(np.abs(radecs.galactic.b.deg) <= 10.0)[0]
 
         double_in_plane_pixels = []
@@ -1128,16 +1135,17 @@
             self.first_obs = Time(min(times), format="jd")
             self.first_obs.utc.format = "isot"
             self.last_obs = Time(max(times), format="jd")
             self.last_obs.utc.format = "isot"
 
         except ValueError:
             err = (
-                f"No observations of this field were found at any time between {self.t_min} and"
-                f"{times[-1]}. Coverage overlap is 0%, but recent observations might be missing!"
+                f"No observations of this event were found at any time between "
+                f"{self.t_min} and {self.t_min + first_det_window_days * u.day}. "
+                f"Coverage overlap is 0%!"
             )
             self.logger.error(err)
             raise ValueError(err)
 
         self.logger.info(f"Observations started at {self.first_obs.isot}")
 
         return (
@@ -1268,19 +1276,19 @@
         gray_patch = mpatches.Patch(color="gray", label="Observed once")
         violet_patch = mpatches.Patch(
             color="green", label="Observed Galactic Plane (|b|<10)"
         )
         plt.legend(handles=[red_patch, gray_patch, violet_patch])
 
         message = (
-            "In total, {0:.2f} % of the contour was observed at least once.\n"
-            "This estimate includes {1:.2f} % of the contour "
+            "In total, {0:.1f} % of the contour was observed at least once.\n"
+            "This estimate includes {1:.1f} % of the contour "
             "at a galactic latitude <10 deg.\n"
-            "In total, {2:.2f} % of the contour was observed at least twice. \n"
-            "In total, {3:.2f} % of the contour was observed at least twice, "
+            "In total, {2:.1f} % of the contour was observed at least twice. \n"
+            "In total, {3:.1f} % of the contour was observed at least twice, "
             "and excluding low galactic latitudes.\n"
             "These estimates account for chip gaps.".format(
                 100
                 * (
                     np.sum(double_in_plane_probs)
                     + np.sum(single_in_plane_prob)
                     + np.sum(single_no_plane_prob)
@@ -1382,20 +1390,20 @@
             res = df[df["field_id"] == field_entry]
 
             mask = res["exposure_time"].astype(float) > 30.0
 
             new = {
                 "field_id": field_entry,
                 "n_exposures": len(res),
-                "n_30": np.sum(mask),
-                "n_deep": np.sum(~mask),
-                "f_proc_30": np.mean(res[mask]["f_processed"]),
-                "f_proc_deep": np.mean(res[~mask]["f_processed"]),
-                "f_proc_without_flag_30": np.mean(res[mask]["f_proc_without_flag"]),
-                "f_proc_without_flag_deep": np.mean(res[~mask]["f_proc_without_flag"]),
+                "n_deep": np.sum(mask),
+                "n_30": np.sum(~mask),
+                "f_proc_deep": np.mean(res[mask]["f_processed"]),
+                "f_proc_30": np.mean(res[~mask]["f_processed"]),
+                "f_proc_without_flag_deep": np.mean(res[mask]["f_proc_without_flag"]),
+                "f_proc_without_flag_30": np.mean(res[~mask]["f_proc_without_flag"]),
                 "n_filters": len(res["filter_id"].unique()),
                 "n_nights": len(set([int(x + 0.5) for x in res["obsjd"]])),
             }
             fields.append(new)
 
         summary = pd.DataFrame(fields)
```

### Comparing `nuztf-2.7.0/nuztf/cat_match.py` & `nuztf-2.7.1/nuztf/cat_match.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/credentials.py` & `nuztf-2.7.1/nuztf/credentials.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/flatpix.py` & `nuztf-2.7.1/nuztf/flatpix.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/fritz.py` & `nuztf-2.7.1/nuztf/fritz.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/irsa.py` & `nuztf-2.7.1/nuztf/irsa.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/neutrino_scanner.py` & `nuztf-2.7.1/nuztf/neutrino_scanner.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/observations.py` & `nuztf-2.7.1/nuztf/observations.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/observations_depot.py` & `nuztf-2.7.1/nuztf/observations_depot.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/parse_nu_gcn.py` & `nuztf-2.7.1/nuztf/parse_nu_gcn.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/paths.py` & `nuztf-2.7.1/nuztf/paths.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/plot.py` & `nuztf-2.7.1/nuztf/plot.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/skymap.py` & `nuztf-2.7.1/nuztf/skymap.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.io import fits
 from astropy.time import Time
 from astropy_healpix import HEALPix
 from ligo.gracedb.exceptions import HTTPError
 from ligo.gracedb.rest import GraceDb
+from ligo.skymap.io import read_sky_map
 from ligo.skymap.moc import rasterize
 from lxml import html
 from numpy.lib.recfunctions import append_fields
 
 from nuztf.paths import RESULTS_DIR, SKYMAP_DIR
 
 
@@ -258,60 +259,61 @@
                     t_obs_mjd = x.header["EVENTMJD"]
                     t_obs = Time(t_obs_mjd, format="mjd").isot
 
                 if "ORDERING" in x.header:
                     ordering = x.header["ORDERING"]
 
         if "PROB" in data.dtype.names:
-            key = "PROB"
-        elif "PROBABILITY" in data.dtype.names:
-            key = "PROB"
-            prob = np.array(data["PROBABILITY"]).flatten()
+            pass
+        elif (replacekey := "PROBABILITY") in data.dtype.names:
+            prob = np.array(data[replacekey]).flatten()
             data = append_fields(data, "PROB", prob)
-        elif "PROBDENSITY" in data.dtype.names:
-            key = "PROB"
-            prob = np.array(data["PROBDENSITY"])
+        elif (replacekey := "PROBDENSITY") in data.dtype.names:
+            prob = np.array(data[replacekey])
             data = append_fields(data, "PROB", prob)
-        elif "T" in data.dtype.names:  # weird IceCube format
-            key = "PROB"
-            prob = np.array(data["T"]).flatten()
+        elif (replacekey := "T") in data.dtype.names:  # weird IceCube format
+            prob = np.array(data[replacekey]).flatten()
             data = append_fields(data, "PROB", prob)
         else:
             raise Exception(
                 f"No recognised probability key in map. This is probably a weird one, right? "
                 f"Found the following keys: {data.dtype.names}"
             )
 
         if ordering == "NUNIQ":
             self.logger.info("Rasterising skymap to convert to nested format")
-            data = data[list(["UNIQ", key])]
-            probs = rasterize(data, order=7)
-            data = np.array(probs, dtype=np.dtype([("PROB", float)]))
+            # We need to use the ligo.skymap.io map parser to make rasterize work
+            skymap_uniq = read_sky_map(self.skymap_path, moc=True)
+            if (replacekey := "PROBDENSITY") in skymap_uniq.colnames:
+                skymap_uniq[replacekey].name = "PROB"
+
+            data = rasterize(skymap_uniq, order=7)
 
         if not isinstance(data["PROB"][0], float):
             self.logger.info("Flattening skymap")
-            probs = np.array(data["PROB"]).flatten()
-            data = np.array(probs, dtype=np.dtype([("PROB", float)]))
+            prob = np.array(data["PROB"]).flatten()
+            data = np.array(prob, dtype=np.dtype([("PROB", float)]))
 
         if "NSIDE" not in h.keys():
-            h["NSIDE"] = hp.npix2nside(len(data[key]))
+            h["NSIDE"] = hp.npix2nside(len(data["PROB"]))
 
         data["PROB"] /= np.sum(data["PROB"])
 
         self.logger.info(f"Summed probability is {100. * np.sum(data['PROB']):.1f}%")
 
         if ordering == "RING":
             data["PROB"] = hp.pixelfunc.reorder(data["PROB"], inp="RING", out="NESTED")
 
         if ordering is not None:
             h["ORDERING"] = "NESTED"
+
         else:
             raise Exception(
                 f"Error parsing fits file, no ordering found. "
-                f"Please enter the ordewring (NESTED/RING/NUNIQ)"
+                f"Please enter the ordering (NESTED/RING/NUNIQ)"
             )
 
         # Optionally interpolate to a different nside
         if output_nside is not None:
             if output_nside != hp.npix2nside(len(data["PROB"])):
                 self.logger.info(f"Regridding to nside {output_nside}")
 
@@ -349,15 +351,15 @@
                 data = new_data
 
         else:
             output_nside = h["NSIDE"]
 
         hpm = HEALPix(nside=output_nside, order="NESTED", frame="icrs")
 
-        return data, t_obs, hpm, key, dist, dist_unc
+        return data, t_obs, hpm, "PROB", dist, dist_unc
 
     def find_pixel_threshold(self, data):
         """
         Find the pixel threshold that corresponds to the probability threshold
 
         :param data: Healpix map data
         :return: threshold value
```

### Comparing `nuztf-2.7.0/nuztf/skymap_scanner.py` & `nuztf-2.7.1/nuztf/skymap_scanner.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/style.py` & `nuztf-2.7.1/nuztf/style.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/nuztf/utils.py` & `nuztf-2.7.1/nuztf/utils.py`

 * *Files identical despite different names*

### Comparing `nuztf-2.7.0/pyproject.toml` & `nuztf-2.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuztf"
-version = "2.7.0"
+version = "2.7.1"
 description = "Package for multi-messenger correlation searches with ZTF"
 authors = ["Robert Stein <rdstein@caltech.edu>", "Simeon Reusch <simeon.reusch@desy.de>", "Jannis Necker <jannis.necker@desy.de>"]
 repository = "https://github.com/desy-multimessenger/nuztf"
 license = "MIT"
 readme = "README.md"
 classifiers = [
         "Operating System :: OS Independent",
```

### Comparing `nuztf-2.7.0/PKG-INFO` & `nuztf-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuztf
-Version: 2.7.0
+Version: 2.7.1
 Summary: Package for multi-messenger correlation searches with ZTF
 Home-page: https://github.com/desy-multimessenger/nuztf
 License: MIT
 Author: Robert Stein
 Author-email: rdstein@caltech.edu
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

