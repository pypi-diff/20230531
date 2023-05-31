# Comparing `tmp/bactopia-1.0.2.tar.gz` & `tmp/bactopia-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bactopia-1.0.2.tar", max compression
+gzip compressed data, was "bactopia-1.0.3.tar", max compression
```

## Comparing `bactopia-1.0.2.tar` & `bactopia-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-04-25 18:04:35.882807 bactopia-1.0.2/LICENSE
--rw-r--r--   0        0        0    27493 2023-04-25 18:04:35.886807 bactopia-1.0.2/README.md
--rw-r--r--   0        0        0      113 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/__init__.py
--rw-r--r--   0        0        0     2667 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/citations.py
--rw-r--r--   0        0        0     5118 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/datasets.py
--rw-r--r--   0        0        0    19341 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/download.py
--rw-r--r--   0        0        0     2416 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/jsonify.py
--rw-r--r--   0        0        0    16397 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/prepare.py
--rw-r--r--   0        0        0    20687 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/search.py
--rw-r--r--   0        0        0    15455 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/summary.py
--rw-r--r--   0        0        0     1398 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parse.py
--rw-r--r--   0        0        0      267 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/__init__.py
--rw-r--r--   0        0        0      484 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/amrfinderplus.py
--rw-r--r--   0        0        0     1000 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/annotator.py
--rw-r--r--   0        0        0     2783 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/ariba.py
--rw-r--r--   0        0        0      664 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/assembler.py
--rw-r--r--   0        0        0     4673 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/blast.py
--rw-r--r--   0        0        0     1365 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/error.py
--rw-r--r--   0        0        0      372 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/gather.py
--rw-r--r--   0        0        0     1492 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/generic.py
--rw-r--r--   0        0        0     2683 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/mapping.py
--rw-r--r--   0        0        0      640 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/mlst.py
--rw-r--r--   0        0        0     1599 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/parsables.py
--rw-r--r--   0        0        0     3093 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/qc.py
--rw-r--r--   0        0        0     5014 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/sketcher.py
--rw-r--r--   0        0        0     2574 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/variants.py
--rw-r--r--   0        0        0      874 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/versions.py
--rw-r--r--   0        0        0     5292 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/summary.py
--rw-r--r--   0        0        0     4496 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/utils.py
--rw-r--r--   0        0        0     1053 2023-04-25 18:04:35.886807 bactopia-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    29090 1970-01-01 00:00:00.000000 bactopia-1.0.2/setup.py
--rw-r--r--   0        0        0    28447 1970-01-01 00:00:00.000000 bactopia-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-31 04:39:04.837370 bactopia-1.0.3/LICENSE
+-rw-r--r--   0        0        0    27493 2023-05-31 04:39:04.837370 bactopia-1.0.3/README.md
+-rw-r--r--   0        0        0      113 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/__init__.py
+-rw-r--r--   0        0        0     2667 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/citations.py
+-rw-r--r--   0        0        0     5118 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/datasets.py
+-rw-r--r--   0        0        0    19341 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/download.py
+-rw-r--r--   0        0        0     2416 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/jsonify.py
+-rw-r--r--   0        0        0    16397 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/prepare.py
+-rw-r--r--   0        0        0    20125 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/search.py
+-rw-r--r--   0        0        0    15455 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/summary.py
+-rw-r--r--   0        0        0     1398 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parse.py
+-rw-r--r--   0        0        0      267 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/__init__.py
+-rw-r--r--   0        0        0      484 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/amrfinderplus.py
+-rw-r--r--   0        0        0     1000 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/annotator.py
+-rw-r--r--   0        0        0     2783 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/ariba.py
+-rw-r--r--   0        0        0      664 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/assembler.py
+-rw-r--r--   0        0        0     4673 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/blast.py
+-rw-r--r--   0        0        0     1365 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/error.py
+-rw-r--r--   0        0        0      372 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/gather.py
+-rw-r--r--   0        0        0     1492 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/generic.py
+-rw-r--r--   0        0        0     2683 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/mapping.py
+-rw-r--r--   0        0        0      640 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/mlst.py
+-rw-r--r--   0        0        0     1599 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/parsables.py
+-rw-r--r--   0        0        0     3093 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/qc.py
+-rw-r--r--   0        0        0     5014 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/sketcher.py
+-rw-r--r--   0        0        0     2574 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/variants.py
+-rw-r--r--   0        0        0      874 2023-05-31 04:39:04.841370 bactopia-1.0.3/bactopia/parsers/versions.py
+-rw-r--r--   0        0        0     5292 2023-05-31 04:39:04.841370 bactopia-1.0.3/bactopia/summary.py
+-rw-r--r--   0        0        0     4496 2023-05-31 04:39:04.841370 bactopia-1.0.3/bactopia/utils.py
+-rw-r--r--   0        0        0     1034 2023-05-31 04:39:04.841370 bactopia-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    29064 1970-01-01 00:00:00.000000 bactopia-1.0.3/setup.py
+-rw-r--r--   0        0        0    28407 1970-01-01 00:00:00.000000 bactopia-1.0.3/PKG-INFO
```

### Comparing `bactopia-1.0.2/LICENSE` & `bactopia-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/README.md` & `bactopia-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/cli/citations.py` & `bactopia-1.0.3/bactopia/cli/citations.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/cli/datasets.py` & `bactopia-1.0.3/bactopia/cli/datasets.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/cli/download.py` & `bactopia-1.0.3/bactopia/cli/download.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/cli/jsonify.py` & `bactopia-1.0.3/bactopia/cli/jsonify.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/cli/prepare.py` & `bactopia-1.0.3/bactopia/cli/prepare.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/cli/search.py` & `bactopia-1.0.3/bactopia/cli/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 import logging
 import random
 import re
 import sys
 from pathlib import Path
 
+import pandas as pd
 import requests
 import rich
 import rich.console
 import rich.traceback
 import rich_click as click
-from pysradb import SRAweb
 from rich.logging import RichHandler
 
 import bactopia
 from bactopia.utils import get_ncbi_genome_size
 
 # Set up Rich
 stderr = rich.console.Console(stderr=True)
@@ -26,14 +26,15 @@
         {
             "name": "Query Options",
             "options": [
                 "--exact-taxon",
                 "--limit",
                 "--accession-limit",
                 "--biosample-subset",
+                "--include-empty",
             ],
         },
         {
             "name": "Filtering Options",
             "options": [
                 "--min-base-count",
                 "--min-read-length",
@@ -51,113 +52,52 @@
                 "--silent",
                 "--version",
                 "--help",
             ],
         },
     ]
 }
-
-
 ENA_URL = "https://www.ebi.ac.uk/ena/portal/api/search"
-FIELDS = [
-    "study_accession",
-    "secondary_study_accession",
-    "sample_accession",
-    "secondary_sample_accession",
-    "experiment_accession",
-    "run_accession",
-    "submission_accession",
-    "tax_id",
-    "scientific_name",
-    "instrument_platform",
-    "instrument_model",
-    "library_name",
-    "library_layout",
-    "nominal_length",
-    "library_strategy",
-    "library_source",
-    "library_selection",
-    "read_count",
-    "base_count",
-    "center_name",
-    "first_public",
-    "last_updated",
-    "experiment_title",
-    "study_title",
-    "study_alias",
-    "experiment_alias",
-    "run_alias",
-    "fastq_bytes",
-    "fastq_md5",
-    "fastq_ftp",
-    "fastq_aspera",
-    "fastq_galaxy",
-    "submitted_bytes",
-    "submitted_md5",
-    "submitted_ftp",
-    "submitted_aspera",
-    "submitted_galaxy",
-    "submitted_format",
-    "sra_bytes",
-    "sra_md5",
-    "sra_ftp",
-    "sra_aspera",
-    "sra_galaxy",
-    "cram_index_ftp",
-    "cram_index_aspera",
-    "cram_index_galaxy",
-    "sample_alias",
-    "broker_name",
-    "sample_title",
-    "first_created",
-]
 
 
-def get_sra_metadata(query: str) -> list:
-    """Fetch metadata from SRA.
+def get_ena_metadata(query: str, is_accession: bool, limit: int):
+    """Fetch metadata from ENA.
+    https://docs.google.com/document/d/1CwoY84MuZ3SdKYocqssumghBF88PWxUZ/edit#heading=h.ag0eqy2wfin5
+
     Args:
-        query (str): The accession to search for.
+        query (str): The query to search for.
+        is_accession (bool): If the query is an accession or not.
+        limit (int): The maximum number of records to return.
+
     Returns:
         list: Records associated with the accession.
     """
-    #
-    db = SRAweb()
-    df = db.search_sra(
-        query, detailed=True, sample_attribute=True, expand_sample_attributes=True
-    )
-    if df is None:
-        return [False, []]
-    return [True, df.to_dict(orient="records")]
-
-
-def get_ena_metadata(query, is_accession, limit=1000000):
-    """USE ENA's API to retrieve the latest results."""
-    # ENA browser info: http://www.ebi.ac.uk/ena/about/browser
     data = {
         "dataPortal": "ena",
         "dccDataOnly": "false",
         "download": "false",
         "result": "read_run",
         "format": "tsv",
         "limit": limit,
-        "fields": ",".join(FIELDS),
+        "fields": "all",
     }
 
     if is_accession:
         data["includeAccessions"] = query
     else:
         data["query"] = (
             f'"{query} AND library_source=GENOMIC AND '
             "(library_strategy=OTHER OR library_strategy=WGS OR "
             "library_strategy=WGA) AND (library_selection=MNase OR "
             "library_selection=RANDOM OR library_selection=unspecified OR "
             'library_selection="size fractionation")"'
         )
 
     headers = {"accept": "*/*", "Content-type": "application/x-www-form-urlencoded"}
+
     r = requests.post(ENA_URL, headers=headers, data=data)
     if r.status_code == requests.codes.ok:
         data = []
         col_names = None
         for line in r.text.split("\n"):
             cols = line.rstrip().split("\t")
             if line:
@@ -166,45 +106,41 @@
                 else:
                     col_names = cols
         return [True, data]
     else:
         return [False, [r.status_code, r.text]]
 
 
-def get_metadata(
-    query: str, ena_query: str, is_accession: bool, limit: int = 1000000
+def get_run_info(
+    sra_query: str, ena_query: str, is_accession: bool, limit: int = 1000000
 ) -> tuple:
     """Retrieve a list of samples available from ENA.
 
     The first attempt will be against ENA, and if that fails, SRA will be queried. This should
     capture those samples not yet synced between ENA and SRA.
 
     Args:
-        query (str): The original query.
+        sra_query (str): A formatted query for SRA searches.
         ena_query (str): A formatted query for ENA searches.
         is_accession (bool): If the query is an accession or not.
         limit (int): The maximum number of records to return.
 
     Returns:
         tuple: Records associated with the accession.
     """
+
     logging.debug("Querying ENA for metadata...")
-    success, ena_data = get_ena_metadata(ena_query, is_accession, limit)
+    success, ena_data = get_ena_metadata(ena_query, is_accession, limit=limit)
     if success:
-        return ena_data
+        return success, ena_data
     else:
-        logging.debug("Failed to get metadata from ENA. Trying SRA...")
-        success, sra_data = get_sra_metadata(query)
-        if not success:
-            logging.error("There was an issue querying ENA and SRA, exiting...")
-            logging.error(f"STATUS: {ena_data[0]}")
-            logging.error(f"TEXT: {ena_data[1]}")
-            sys.exit(1)
-        else:
-            return sra_data
+        logging.error("There was an issue querying ENA, exiting...")
+        logging.error(f"STATUS: {ena_data[0]}")
+        logging.error(f"TEXT: {ena_data[1]}")
+        sys.exit(1)
 
 
 def parse_accessions(
     results: dict,
     min_read_length: int,
     min_base_count: int,
     genome_size: int,
@@ -227,22 +163,25 @@
     filtered = {
         "min_base_count": 0,
         "min_read_length": 0,
         "technical": 0,
         "filtered": [],
     }
     for result in results:
+        instrument_key = (
+            "instrument_platform"
+            if "instrument_platform" in result
+            else "instrument_model_desc"
+        )
         if (
-            result["instrument_platform"] == "ILLUMINA"
-            or result["instrument_platform"] == "OXFORD_NANOPORE"
+            result[instrument_key] == "ILLUMINA"
+            or result[instrument_key] == "OXFORD_NANOPORE"
         ):
             technology = (
-                "ont"
-                if result["instrument_platform"] == "OXFORD_NANOPORE"
-                else "illumina"
+                "ont" if result[instrument_key] == "OXFORD_NANOPORE" else "illumina"
             )
             passes = True
             reason = []
             if not result["fastq_bytes"]:
                 passes = False
                 reason.append("Missing FASTQs")
                 filtered["technical"] += 1
@@ -325,55 +264,59 @@
                 if line:
                     queries.append(line)
     elif "," in q:
         queries = q.split(",")
     else:
         queries.append(q)
     results = []
+    bioproject_accessions = []
+    biosample_accessions = []
     experiment_accessions = []
     run_accessions = []
 
     for query in queries:
         try:
             taxon_id = int(query)
             if exact_taxon:
-                results.append(["taxon", f"tax_eq({taxon_id})"])
+                results.append(
+                    ["taxon", f"tax_eq({taxon_id})", f"txid{taxon_id}[Organism:noexp]"]
+                )
             else:
-                results.append(["taxon_tree", f"tax_tree({taxon_id})"])
+                results.append(
+                    [
+                        "taxon_tree",
+                        f"tax_tree({taxon_id})",
+                        f"txid{taxon_id}[Organism:exp]",
+                    ]
+                )
         except ValueError:
             # It is a accession or scientific name
             # Test Accession
             # Thanks! https://ena-docs.readthedocs.io/en/latest/submit/general-guide/accessions.html#accession-numbers
             if re.match(r"^PRJ[EDN][A-Z][0-9]+$|^[EDS]RP[0-9]{6,}$", query):
-                results.append(
-                    [
-                        "bioproject",
-                        f"(study_accession={query} OR secondary_study_accession={query})",
-                    ]
-                )
+                bioproject_accessions.append(query)
             elif re.match(r"^SAM[EDN][A-Z]?[0-9]+$|^[EDS]RS[0-9]{6,}$", query):
-                results.append(
-                    [
-                        "biosample",
-                        f"(sample_accession={query} OR secondary_sample_accession={query})",
-                    ]
-                )
+                biosample_accessions.append(query)
             elif re.match(r"^[EDS]RX[0-9]{6,}$", query):
                 experiment_accessions.append(query)
             elif re.match(r"^[EDS]RR[0-9]{6,}$", query):
                 run_accessions.append(query)
             else:
                 # Assuming it is a scientific name
-                results.append(["taxon_name", f'tax_name("{query}")'])
+                results.append(["taxon_name", f'tax_name("{query}")', f"'{query}'"])
 
     # Split the accessions into set number
+    for chunk in chunks(bioproject_accessions, accession_limit):
+        results.append(["bioproject_accession", ",".join(chunk), " OR ".join(chunk)])
+    for chunk in chunks(biosample_accessions, accession_limit):
+        results.append(["biosample_accession", ",".join(chunk), " OR ".join(chunk)])
     for chunk in chunks(experiment_accessions, accession_limit):
-        results.append(["experiment_accession", ",".join(chunk)])
+        results.append(["experiment_accession", ",".join(chunk), " OR ".join(chunk)])
     for chunk in chunks(run_accessions, accession_limit):
-        results.append(["run_accession", ",".join(chunk)])
+        results.append(["run_accession", ",".join(chunk), " OR ".join(chunk)])
 
     return results
 
 
 @click.command()
 @click.version_option(bactopia.__version__, "--version", "-V")
 @click.option(
@@ -437,14 +380,19 @@
 @click.option(
     "--genome-size",
     "-gsize",
     default=0,
     show_default=True,
     help="Genome size to be used for all samples, and for calculating min coverage",
 )
+@click.option(
+    "--include-empty",
+    is_flag=True,
+    help="Include metadata columns that are empty for all rows",
+)
 @click.option("--force", is_flag=True, help="Overwrite existing reports")
 @click.option("--verbose", is_flag=True, help="Increase the verbosity of output")
 @click.option("--silent", is_flag=True, help="Only critical errors will be printed")
 def search(
     query,
     exact_taxon,
     outdir,
@@ -452,14 +400,15 @@
     limit,
     accession_limit,
     biosample_subset,
     min_base_count,
     min_read_length,
     min_coverage,
     genome_size,
+    include_empty,
     force,
     verbose,
     silent,
 ):
     """Query against ENA and SRA for public accessions to process with Bactopia"""
     # Setup logs
     logging.basicConfig(
@@ -474,31 +423,31 @@
     )
 
     # if not os.path.exists(args.outdir):
     #    os.makedirs(args.outdir, exist_ok=True)
 
     if min_coverage and genome_size:
         if min_base_count:
-            print(
+            logging.error(
                 "--min_base_count cannot be used with --coverage/--genome_size. Exiting...",
                 file=sys.stderr,
             )
             sys.exit(1)
         else:
             min_base_count = min_coverage * genome_size
     elif min_coverage or genome_size:
-        print(
+        logging.error(
             "--coverage and --genome_size must be used together. Exiting...",
             file=sys.stderr,
         )
         sys.exit(1)
 
     if biosample_subset > 0:
         if not is_biosample(query):
-            print(
+            logging.error(
                 "--biosample_subset requires a single BioSample. Input query: {query} is not a BioSample. Exiting...",
                 file=sys.stderr,
             )
             sys.exit(1)
 
     results = []
 
@@ -515,18 +464,20 @@
 
     # Output files
     metadata_file = f"{outdir}/{prefix}-metadata.txt".replace("//", "/")
     accessions_file = f"{outdir}/{prefix}-accessions.txt".replace("//", "/")
     filtered_file = f"{outdir}/{prefix}-filtered.txt".replace("//", "/")
     summary_file = f"{outdir}/{prefix}-search.txt".replace("//", "/")
     genome_sizes = get_ncbi_genome_size()
-    for query_type, query in queries:
+    for query_type, ena_query, sra_query in queries:
         logging.info(f"Submitting query (type - {query_type})")
         is_accession = True if query_type.endswith("accession") else False
-        success, query_results = get_ena_metadata(query, is_accession, limit=limit)
+        success, query_results = get_run_info(
+            sra_query, ena_query, is_accession, limit=limit
+        )
         results += query_results
         if success:
             query_accessions, query_filtered = parse_accessions(
                 query_results,
                 min_read_length=min_read_length,
                 min_base_count=min_base_count,
                 genome_size=genome_size,
@@ -598,18 +549,21 @@
             summary.append("")
         else:
             logging.error(f"ERROR: Unable to retrieve metadata for query ({query})")
 
     # Output the results
     logging.info(f"Writing results to {metadata_file}")
     with open(metadata_file, "w") as output_fh:
-        output_fh.write(f"{results[0].keys()}\n")
-        for result in results:
-            if result:
-                output_fh.write(f"{result}\n")
+        df = pd.DataFrame.from_dict(results)
+        if not include_empty:
+            logging.debug(f"Removing empty columns from {metadata_file}")
+            df.replace("", float("NaN"), inplace=True)
+            df.dropna(inplace=True, how="all", axis=1)
+            df.replace(float("NaN"), "", inplace=True)
+        df.to_csv(output_fh, sep="\t", index=False)
 
     logging.info(f"Writing accessions to {accessions_file}")
     with open(accessions_file, "w") as output_fh:
         for accession in accessions:
             output_fh.write(f"{accession}\n")
 
     logging.info(f"Writing filtered accessions to {filtered_file}")
```

### Comparing `bactopia-1.0.2/bactopia/cli/summary.py` & `bactopia-1.0.3/bactopia/cli/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parse.py` & `bactopia-1.0.3/bactopia/parse.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/annotator.py` & `bactopia-1.0.3/bactopia/parsers/annotator.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/ariba.py` & `bactopia-1.0.3/bactopia/parsers/ariba.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/assembler.py` & `bactopia-1.0.3/bactopia/parsers/assembler.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/blast.py` & `bactopia-1.0.3/bactopia/parsers/blast.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/error.py` & `bactopia-1.0.3/bactopia/parsers/error.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/generic.py` & `bactopia-1.0.3/bactopia/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/mapping.py` & `bactopia-1.0.3/bactopia/parsers/mapping.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/mlst.py` & `bactopia-1.0.3/bactopia/parsers/mlst.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/parsables.py` & `bactopia-1.0.3/bactopia/parsers/parsables.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/qc.py` & `bactopia-1.0.3/bactopia/parsers/qc.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/sketcher.py` & `bactopia-1.0.3/bactopia/parsers/sketcher.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/variants.py` & `bactopia-1.0.3/bactopia/parsers/variants.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/parsers/versions.py` & `bactopia-1.0.3/bactopia/parsers/versions.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/summary.py` & `bactopia-1.0.3/bactopia/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/bactopia/utils.py` & `bactopia-1.0.3/bactopia/utils.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.2/pyproject.toml` & `bactopia-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bactopia"
-version = "1.0.2"
+version = "1.0.3"
 description = "A Python package for working with Bactopia"
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://bactopia.github.io/"
@@ -22,15 +22,14 @@
 [tool.poetry.dependencies]
 python = "^3.8.0"
 requests = "^2.28.2"
 rich-click = "^1.6.1"
 executor = "^23.2"
 rich = "^13.3.1"
 pandas = "^1.5.3"
-pysradb = "^1.4.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.0"
 flake8 = "^5.0"
 
 [tool.isort]
```

### Comparing `bactopia-1.0.2/setup.py` & `bactopia-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,29 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['executor>=23.2,<24.0',
  'pandas>=1.5.3,<2.0.0',
- 'pysradb>=1.4.2,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'rich-click>=1.6.1,<2.0.0',
  'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['bactopia-citations = bactopia.cli.citations:main',
                      'bactopia-datasets = bactopia.cli.datasets:main',
                      'bactopia-download = bactopia.cli.download:main',
                      'bactopia-prepare = bactopia.cli.prepare:main',
                      'bactopia-search = bactopia.cli.search:main',
                      'bactopia-summary = bactopia.cli.summary:main']}
 
 setup_kwargs = {
     'name': 'bactopia',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'A Python package for working with Bactopia',
     'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version        -V        Show the version and exit.                             │\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │\n│                               [required]                                             │\n│    --name           -n  TEXT  Only print citation matching a given name              │\n│    --plain-text     -p        Disable rich formatting                                │\n│    --help                     Show this message and exit.                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-datasets`\n\n```{bash}\n Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...\n\n Download optional datasets to supplement your analyses with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Download Related Options ───────────────────────────────────────────────────────────╮\n│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │\n│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │\n│                              will be created)                                        │\n│                              [default: ${HOME}/.bactopia]                 │\n│ --force                      Force overwrite of existing pre-built environments.     │\n│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │\n│                              (Default: 3)                                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bactopia.github.io/',
```

### Comparing `bactopia-1.0.2/PKG-INFO` & `bactopia-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bactopia
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for working with Bactopia
 Home-page: https://bactopia.github.io/
 License: MIT
 Keywords: bioinformatics,bacteria,bactopia,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: executor (>=23.2,<24.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pysradb (>=1.4.2,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Project-URL: Repository, https://github.com/bactopia/bactopia-py
 Description-Content-Type: text/markdown
 
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)
```

