# Comparing `tmp/ontogpt-0.2.7.tar.gz` & `tmp/ontogpt-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.7.tar", max compression
+gzip compressed data, was "ontogpt-0.2.8.tar", max compression
```

## Comparing `ontogpt-0.2.7.tar` & `ontogpt-0.2.8.tar`

### file list

```diff
@@ -1,112 +1,125 @@
--rw-r--r--   0        0        0     1485 2023-05-18 20:56:47.378187 ontogpt-0.2.7/LICENSE
--rw-r--r--   0        0        0    13196 2023-05-18 20:56:47.378187 ontogpt-0.2.7/README.md
--rw-r--r--   0        0        0     2417 2023-05-18 20:57:52.962670 ontogpt-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    32669 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     6962 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2921 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1122 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0      684 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/conf/synonymizer-conf.yaml
--rw-r--r--   0        0        0       81 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5289 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/embedding_similarity_engine.py
--rw-r--r--   0        0        0    12456 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/enrichment.py
--rw-r--r--   0        0        0    19185 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    24196 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      752 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    18520 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      719 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-05-18 20:56:47.422188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10390 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10670 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/enrichment/__init__.py
--rw-r--r--   0        0        0    13726 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/enrichment/eval_enrichment.py
--rw-r--r--   0        0        0     2950 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6164 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8973 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1191 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rw-r--r--   0        0        0     4791 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
--rwxr-xr-x   0        0        0       95 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0      586 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      386 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4329 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3255 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2350 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1440 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0      899 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/__init__.py
--rw-r--r--   0        0        0      159 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
--rw-r--r--   0        0        0     1016 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
--rw-r--r--   0        0        0      993 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
--rw-r--r--   0        0        0      994 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
--rw-r--r--   0        0        0      995 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
--rw-r--r--   0        0        0      560 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/prompts/similarity/connections.jinja2
--rw-r--r--   0        0        0     2354 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/streamlit/spindoctor.py
--rw-r--r--   0        0        0       68 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0     5942 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     2938 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.yaml
--rw-r--r--   0        0        0     4519 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/composite_disease.yaml
--rw-r--r--   0        0        0     3593 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3445 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6210 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     8878 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.py
--rw-r--r--   0        0        0     4774 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.yaml
--rw-r--r--   0        0        0     5466 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6092 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2900 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     4709 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1614 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     8172 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6813 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     8165 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     6097 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5384 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7156 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5072 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     6136 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.py
--rw-r--r--   0        0        0     3383 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.yaml
--rw-r--r--   0        0        0     4887 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7501 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7222 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-05-18 20:56:47.426188 ontogpt-0.2.7/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     5467 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/traits.py
--rw-r--r--   0        0        0     3502 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/traits.yaml
--rw-r--r--   0        0        0     7847 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/utils/__init__.py
--rw-r--r--   0        0        0     8799 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/utils/gene_set_utils.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2767 2023-05-18 20:56:47.430188 ontogpt-0.2.7/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    15658 1970-01-01 00:00:00.000000 ontogpt-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-05-31 01:01:27.156528 ontogpt-0.2.8/LICENSE
+-rw-r--r--   0        0        0    13196 2023-05-31 01:01:27.156528 ontogpt-0.2.8/README.md
+-rw-r--r--   0        0        0     2649 2023-05-31 01:02:30.101659 ontogpt-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    36466 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6975 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0    12490 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    24946 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0    10762 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/mapping_engine.py
+-rw-r--r--   0        0        0     1112 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/models.py
+-rw-r--r--   0        0        0    11110 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/reasoner_engine.py
+-rw-r--r--   0        0        0      752 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    18526 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-05-31 01:01:27.204529 ontogpt-0.2.8/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    13787 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0     1346 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/csv_wrapper.py
+-rw-r--r--   0        0        0      386 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0     1742 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/ontex/__init__.py
+-rw-r--r--   0        0        0    57127 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/ontex/extractor.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0     1016 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      993 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
+-rw-r--r--   0        0        0      994 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
+-rw-r--r--   0        0        0      995 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
+-rw-r--r--   0        0        0      152 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/mapping/__init__.py
+-rw-r--r--   0        0        0     2424 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/mapping/eval-mapping.jinja2
+-rw-r--r--   0        0        0      150 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/reasoning/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/reasoning/reasoning.jinja2
+-rw-r--r--   0        0        0      560 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0     2353 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/streamlit/spindoctor.py
+-rw-r--r--   0        0        0       68 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0     5942 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     5061 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/biotic_interaction.py
+-rw-r--r--   0        0        0     1886 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/biotic_interaction.yaml
+-rw-r--r--   0        0        0     2938 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     4519 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/composite_disease.yaml
+-rw-r--r--   0        0        0     3593 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3446 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     8878 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/diagnostic_procedure.py
+-rw-r--r--   0        0        0     4774 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/diagnostic_procedure.yaml
+-rw-r--r--   0        0        0     5466 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     3147 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1614 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-05-31 01:01:27.208529 ontogpt-0.2.8/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     6136 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/ontology_issue.py
+-rw-r--r--   0        0        0     3383 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/ontology_issue.yaml
+-rw-r--r--   0        0        0     4887 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     5511 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/traits.py
+-rw-r--r--   0        0        0     3502 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/traits.yaml
+-rw-r--r--   0        0        0     7847 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     8799 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/utils/gene_set_utils.py
+-rw-r--r--   0        0        0      283 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/utils/parse_utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2877 2023-05-31 01:01:27.212529 ontogpt-0.2.8/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    15887 1970-01-01 00:00:00.000000 ontogpt-0.2.8/PKG-INFO
```

### Comparing `ontogpt-0.2.7/LICENSE` & `ontogpt-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/README.md` & `ontogpt-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/pyproject.toml` & `ontogpt-0.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.7"
+version = "0.2.8"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
@@ -14,41 +14,44 @@
 oaklib = "^0.5.6"
 gilda = "^0.10.3"
 jsonlines = "^3.1.0"
 python-multipart = "^0.0.5"
 linkml-owl = "^0.2.7"
 beautifulsoup4 = "^4.11.1"
 eutils = "^0.6.0"
-class-resolver = "*"
+class-resolver = ">=0.4.2"
 inflect = "^6.0.2"
 bioc = "^2.0.post5"
 linkml = "^1.4.10"
 wikipedia = "^1.4.0"
 tiktoken = "^0.3.3"
 airium = "^0.2.5"
 SQLAlchemy = "^1.4.32, !=1.4.46"
 greenlet = "!=2.0.2"
 httpx = "^0.23.3"
 aiohttp = "^3.8.4"
 inflection = "^0.5.1"
-linkml-runtime = "^1.4.9"
+linkml-runtime = "^1.5.3"
 nlpcloud = "^1.0.39"
 fastapi = {version = "^0.88.0", optional = true}
 uvicorn = {version = "^0.20.0", optional = true}
 Jinja2 = {version = "^3.1.2", optional = true}
 sphinx = {version = "^5.3.0", extras = ["docs"], optional = true}
 sphinx-rtd-theme = {version = "^1.0.0", extras = ["docs"], optional = true}
 sphinx-autodoc-typehints = {version = "^1.19.4", extras = ["docs"], optional = true}
 sphinx-click = {version = "^4.3.0", extras = ["docs"], optional = true}
 myst-parser = {version = "^0.18.1", extras = ["docs"], optional = true}
 recipe-scrapers = {version = "^14.35.0", extras = ["recipes"], optional = true}
+textract = {version = "*", extras = ["textract"], optional = true}
 cachier = "^2.1.0"
 wikipedia-api = "^0.5.8"
-rustsim = "^0.1.8"
+semsimian = ">=0.1.13"
 requests-cache = "^1.0.1"
+langchain = "^0.0.167"
+pygpt4all = {version = "^1.1.0", extras = ["gpt4all"], optional = true}
 streamlit = "^1.22.0"
 gpt4 = "^0.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 setuptools = ">=65.5.0"
 tox = "^3.25.1"
@@ -70,14 +73,20 @@
     "fastapi",
     "uvicorn",
     "Jinja2"
 ]
 recipes = [
     "recipe-scrapers"
 ]
+gpt4all = [
+    "pygpt4all"
+]
+textract = [
+    "textract"
+]
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 seaborn = "^0.12.2"
 papermill = "^2.4.0"
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `ontogpt-0.2.7/src/ontogpt/cli.py` & `ontogpt-0.2.8/src/ontogpt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 """Command line interface for oak-ai."""
 import codecs
 import logging
 import pickle
 import sys
-from copy import copy
+from copy import copy, deepcopy
 from dataclasses import dataclass
 from io import BytesIO, TextIOWrapper
 from pathlib import Path
 from typing import List, Optional
 
 import click
 import jsonlines
 import openai
 import yaml
 from oaklib import get_adapter
 from oaklib.cli import query_terms_iterator
+from oaklib.interfaces import OboGraphInterface
 from oaklib.io.streaming_csv_writer import StreamingCsvWriter
 
+import ontogpt.ontex.extractor as extractor
 from ontogpt import __version__
 from ontogpt.clients import OpenAIClient
 from ontogpt.clients.pubmed_client import PubmedClient
 from ontogpt.clients.soup_client import SoupClient
 from ontogpt.clients.wikipedia_client import WikipediaClient
 from ontogpt.engines import create_engine
 from ontogpt.engines.embedding_similarity_engine import SimilarityEngine
 from ontogpt.engines.enrichment import EnrichmentEngine
 from ontogpt.engines.halo_engine import HALOEngine
 from ontogpt.engines.knowledge_engine import KnowledgeEngine
+from ontogpt.engines.mapping_engine import MappingEngine, MappingTaskCollection
+from ontogpt.engines.reasoner_engine import ReasonerEngine
 from ontogpt.engines.spires_engine import SPIRESEngine
 from ontogpt.engines.synonym_engine import SynonymEngine
 from ontogpt.evaluation.enrichment.eval_enrichment import EvalEnrichment
 from ontogpt.evaluation.resolver import create_evaluator
+from ontogpt.io.csv_wrapper import write_obj_as_csv
 from ontogpt.io.html_exporter import HTMLExporter
 from ontogpt.io.markdown_exporter import MarkdownExporter
 from ontogpt.utils.gene_set_utils import (
     GeneSet,
     _is_human,
     fill_missing_gene_set_values,
     parse_gene_set,
@@ -107,31 +112,43 @@
 )
 interactive_option = click.option(
     "--interactive/--no-interactive",
     default=False,
     show_default=True,
     help="Interactive mode - rather than call the LLM API it will prompt you do this.",
 )
-model_option = click.option("-m", "--model", help="Engine to use, e.g. text-davinci-003.")
+model_option = click.option(
+    "-m",
+    "--model",
+    help="Model name to use, e.g. openai-text-davinci-003."
+         " The first part of this name must be the source of the model."
+         " The second part must be the model name.",
+)
 prompt_template_option = click.option(
     "--prompt-template", help="Path to a file containing the prompt."
 )
 recurse_option = click.option(
     "--recurse/--no-recurse", default=True, show_default=True, help="Recursively parse structures."
 )
+use_textract_options = click.option(
+    "--use-textract/--no-use-textract",
+    default=False,
+    show_default=True,
+    help="Use textract to extract text.",
+)
 output_option_wb = click.option(
     "-o", "--output", type=click.File(mode="wb"), default=sys.stdout, help="Output file."
 )
 output_option_txt = click.option(
     "-o", "--output", type=click.File(mode="w"), default=sys.stdout, help="Output file."
 )
 output_format_options = click.option(
     "-O",
     "--output-format",
-    type=click.Choice(["json", "yaml", "pickle", "md", "html", "owl", "turtle"]),
+    type=click.Choice(["json", "yaml", "pickle", "md", "html", "owl", "turtle", "jsonl"]),
     default="yaml",
     help="Output format.",
 )
 
 
 @click.group()
 @click.option("-v", "--verbose", count=True)
@@ -168,14 +185,15 @@
 @template_option
 @target_class_option
 @model_option
 @recurse_option
 @output_option_wb
 @click.option("--dictionary")
 @output_format_options
+@use_textract_options
 @click.option("--auto-prefix", default="AUTO", help="Prefix to use for auto-generated classes.")
 @click.option(
     "--set-slot-value",
     "-S",
     multiple=True,
     help="Set slot value, e.g. --set-slot-value has_participant=protein",
 )
@@ -185,14 +203,15 @@
     template,
     target_class,
     dictionary,
     input,
     output,
     output_format,
     set_slot_value,
+    use_textract,
     **kwargs,
 ):
     """Extract knowledge from text guided by schema, using SPIRES engine.
 
     Example:
 
         ontogpt extract -t gocam.GoCamAnnotations -i gocam-27929086.txt
@@ -214,15 +233,20 @@
     if settings.cache_db:
         ke.client.cache_db_path = settings.cache_db
     if settings.skip_annotators:
         ke.client.skip_annotators = settings.skip_annotators
     if dictionary:
         ke.load_dictionary(dictionary)
     if inputfile and Path(inputfile).exists():
-        text = open(inputfile, "r").read()
+        if use_textract:
+            import textract
+
+            text = textract.process(inputfile).decode("utf-8")
+        else:
+            text = open(inputfile, "r").read()
     elif inputfile and not Path(inputfile).exists():
         raise FileNotFoundError(f"Cannot find input file {inputfile}")
     elif input:
         text = input
     elif not input or input == "-":
         text = sys.stdin.read()
     logging.info(f"Input text: {text}")
@@ -785,14 +809,105 @@
     for e1 in entities1:
         sims = engine.search(e1, entities2)
         for sim in sims:
             writer.emit(sim)
 
 
 @main.command()
+@inputfile_option
+@output_option_txt
+@model_option
+@click.option("--task-file")
+@click.option("--task-type")
+@click.option("--tsv-output")
+@click.option("--all-methods/--no-all-methods", default=False)
+@click.option("--explain/--no-explain", default=False)
+@click.option("--evaluate/--no-evaluate", default=False)
+@click.argument("terms", nargs=-1)
+def reason(
+    terms,
+    inputfile,
+    model,
+    task_file,
+    explain,
+    task_type,
+    output,
+    tsv_output,
+    all_methods,
+    evaluate,
+    **kwargs,
+):
+    """Reason."""
+    reasoner = ReasonerEngine(model=model)
+    if task_file:
+        tc = MappingTaskCollection.load(task_file)
+    else:
+        adapter = get_adapter(inputfile)
+        if not isinstance(adapter, OboGraphInterface):
+            raise ValueError("Only OBO graphs supported")
+        ex = extractor.OntologyExtractor(adapter=adapter)
+        # ex.use_identifiers = True
+        task = ex.create_task(task_type=task_type, parameters=list(terms))
+        tc = extractor.TaskCollection(tasks=[task])
+    if all_methods:
+        tasks = []
+        print(f"Cloning {len(tc.tasks)} tasks")
+        for core_task in tc.tasks:
+            for m in extractor.GPTReasonMethodType:
+                print(f"Cloning {m}")
+                task = deepcopy(core_task)
+                task.method = m
+                task.init_method()
+                tasks.append(task)
+        tc.tasks = tasks
+        print(f"New {len(tc.tasks)} tasks")
+    else:
+        for task in tc.tasks:
+            task.include_explanations = explain
+    resultset = reasoner.reason_multiple(tc, evaluate=evaluate)
+    dump_minimal_yaml(resultset.dict(), file=output)
+    if tsv_output:
+        write_obj_as_csv(resultset.results, tsv_output)
+
+
+@main.command()
+@inputfile_option
+@output_option_txt
+@model_option
+@click.option("--task-file")
+@click.option("--task-type")
+@click.option("--tsv-output")
+@click.option("--all-methods/--no-all-methods", default=False)
+@click.option("--explain/--no-explain", default=False)
+@click.option("--evaluate/--no-evaluate", default=False)
+@click.argument("terms", nargs=-1)
+def categorize_mappings(
+    terms,
+    inputfile,
+    model,
+    task_file,
+    explain,
+    task_type,
+    output,
+    tsv_output,
+    all_methods,
+    evaluate,
+    **kwargs,
+):
+    """Categorize a collection of SSSOM mappings."""
+    mapper = MappingEngine(model=model)
+    tc = mapper.from_sssom(inputfile)
+    for cm in mapper.run_tasks(tc, evaluate=evaluate):
+        print(dump_minimal_yaml(cm.dict()))
+    # dump_minimal_yaml(cm.dict(), file=output)
+    if tsv_output:
+        write_obj_as_csv(resultset.results, tsv_output)
+
+
+@main.command()
 @output_option_txt
 @click.option(
     "--strict/--no-strict",
     default=True,
     show_default=True,
     help="If set, there must be a unique mappings from labels to IDs",
 )
@@ -831,16 +946,17 @@
 #    help="DO NOT USE EXCEPT FOR EVALUATION PUPOSES."
 # )
 @click.option(
     "--annotations-path",
     "-A",
     help="Path to annotations",
 )
+@model_option
 @click.argument("genes", nargs=-1)
-def eval_enrichment(genes, input_file, number_to_drop, annotations_path, output, **kwargs):
+def eval_enrichment(genes, input_file, number_to_drop, annotations_path, model, output, **kwargs):
     """Run enrichment using multiple methods."""
     if not genes and not input_file:
         raise ValueError("Either genes or input file must be passed")
     if genes:
         gene_set = GeneSet(name="TEMP", gene_symbols=genes)
     if input_file:
         if genes:
@@ -849,15 +965,15 @@
     if not gene_set:
         raise ValueError("No genes passed")
     fill_missing_gene_set_values(gene_set)
     if not annotations_path:
         if not _is_human(gene_set):
             raise ValueError("No annotations path passed")
         annotations_path = "tests/input/genes2go.tsv.gz"
-    eval_engine = EvalEnrichment()
+    eval_engine = EvalEnrichment(model=model)
     eval_engine.load_annotations(annotations_path)
     comps = eval_engine.evaluate_methods_on_gene_set(gene_set, n=number_to_drop, **kwargs)
     output.write(dump_minimal_yaml(comps))
 
 
 @main.command()
 @model_option
@@ -899,16 +1015,16 @@
     examples = yaml.safe_load(examples)
     logging.debug(f"Input object: {object}")
     results = ke.generalize(object, examples)
     output.write(yaml.dump(results.dict()))
 
 
 @main.command()
-def models(**kwargs):
-    """Prompt completion."""
+def openai_models(**kwargs):
+    """List OpenAI models for prompt completion."""
     ai = OpenAIClient()
     for model in openai.Model.list():
         print(model)
 
 
 @main.command()
 @model_option
@@ -939,28 +1055,27 @@
 
 @main.command()
 @click.option("-o", "--output", type=click.File(mode="w"), default=sys.stdout, help="Output file.")
 @output_format_options
 @model_option
 @click.option("-m", "match", help="Match string to use for filtering.")
 @click.option("-D", "database", help="Path to sqlite database.")
-def dump_completions(engine, match, database, output, output_format):
+def dump_completions(model, match, database, output, output_format):
     """Dump cached completions."""
-    logging.info(f"Creating for {engine}")
     client = OpenAIClient()
     if database:
         client.cache_db_path = database
     if output_format == "jsonl":
         writer = jsonlines.Writer(output)
-        for engine, prompt, completion in client.cached_completions(match):
-            writer.write(dict(engine=engine, prompt=prompt, completion=completion))
+        for _engine, prompt, completion in client.cached_completions(match):
+            writer.write(dict(engine=model, prompt=prompt, completion=completion))
     elif output_format == "yaml":
-        for engine, prompt, completion in client.cached_completions(match):
+        for _engine, prompt, completion in client.cached_completions(match):
             output.write(
-                dump_minimal_yaml(dict(engine=engine, prompt=prompt, completion=completion))
+                dump_minimal_yaml(dict(engine=model, prompt=prompt, completion=completion))
             )
     else:
         output.write("# Cached Completions:\n")
         for engine, prompt, completion in client.cached_completions(match):
             output.write("## Entry\n")
             output.write(f"### Engine: {engine}\n")
             output.write(f"### Prompt:\n\n {prompt}\n\n")
@@ -1042,9 +1157,20 @@
 
 @main.command()
 def list_templates():
     """List the templates."""
     print("TODO")
 
 
+@main.command()
+def list_models():
+    """List all available models."""
+    print("Model Name\tAlternatives")
+    for modelname in MODELS:
+        if len(modelname) > 1:
+            alternative_names = " ".join(modelname[1:])
+            print(f"{modelname[0]}\t{alternative_names}")
+        else:
+            print(modelname[0])
+
 if __name__ == "__main__":
     main()
```

### Comparing `ontogpt-0.2.7/src/ontogpt/clients/openai_client.py` & `ontogpt-0.2.8/src/ontogpt/clients/openai_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     def __post_init__(self):
         if not self.api_key:
             self.api_key = get_apikey_value("openai")
         openai.api_key = self.api_key
 
     def complete(self, prompt, max_tokens=3000, **kwargs) -> str:
         engine = self.model
-        logging.info(f"Complete: engine={engine}, prompt={prompt[0:100]}...")
+        logger.info(f"Complete: engine={engine}, prompt[{len(prompt)}]={prompt[0:100]}...")
         cur = self.db_connection()
         res = cur.execute("SELECT payload FROM cache WHERE prompt=? AND engine=?", (prompt, engine))
         payload = res.fetchone()
         if payload:
             prompt_peek = str(prompt)[0:80].replace("\n", "\\n")
             logger.info(f"Using cached payload for prompt: {prompt_peek}...")
             return payload[0]
         response = None
         i = 0
         while not response:
             i += 1
-            logging.debug(f"Calling OpenAI API (attempt {i})...")
+            logger.debug(f"Calling OpenAI API (attempt {i})...")
             try:
                 if self.interactive:
                     response = self._interactive_completion(prompt, engine, max_tokens, **kwargs)
                 elif self._must_use_chat_api():
                     response = openai.ChatCompletion.create(
                         model=engine,
                         messages=[
```

### Comparing `ontogpt-0.2.7/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.8/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.8/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.2.8/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/conf/synonymizer-conf.yaml` & `ontogpt-0.2.8/src/ontogpt/conf/synonymizer-conf.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.8/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/embedding_similarity_engine.py` & `ontogpt-0.2.8/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/enrichment.py` & `ontogpt-0.2.8/src/ontogpt/engines/enrichment.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 from jinja2 import Template
 from oaklib import BasicOntologyInterface, get_adapter
 from pydantic import BaseModel
 
-from ontogpt.engines.knowledge_engine import MODEL_GPT_4, KnowledgeEngine
+from ontogpt.engines.knowledge_engine import KnowledgeEngine
+from ontogpt.engines.models import MODEL_GPT_4
 from ontogpt.prompts.enrichment import DEFAULT_ENRICHMENT_PROMPT
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.templates.gene_description_term import GeneDescriptionTerm
 from ontogpt.utils.gene_set_utils import (
     ENTITY_ID,
     GENE_TUPLE,
     GeneSet,
@@ -245,15 +246,15 @@
             END_MARKER=self.end_marker,
         )
         logging.debug(f"Prompt from template: {prompt}")
         logging.info(f"Prompt [{truncation_factor}] Length: {len(prompt)}")
         # https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
         prompt_length = len(self.encoding.encode(prompt)) + 10
         max_len_total = 4097
-        if self.model == MODEL_GPT_4:
+        if self.model in MODEL_GPT_4:
             max_len_total = 8193
         max_len = max_len_total - self.completion_length
         logging.info(
             f"Prompt [{truncation_factor}] Toks: {prompt_length} / {max_len} Str={len(prompt)}"
         )
         if prompt_length > max_len:  # TODO: check this
             logging.warning(f"Prompt is too long; toks: {prompt_length} len: {len(prompt)}")
```

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.8/src/ontogpt/engines/halo_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.8/src/ontogpt/engines/knowledge_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from oaklib.datamodels.text_annotator import TextAnnotationConfiguration
 from oaklib.implementations import OntoPortalImplementationBase
 from oaklib.interfaces import MappingProviderInterface, TextAnnotatorInterface
 from oaklib.utilities.apikey_manager import get_apikey_value
 from oaklib.utilities.subsets.value_set_expander import ValueSetExpander
 
 from ontogpt.clients import OpenAIClient
+from ontogpt.engines.models import DEFAULT_MODEL, GGML_MODELS, MODELS, OPENAI_MODELS
 from ontogpt.templates.core import ExtractionResult, NamedEntity
 
 this_path = Path(__file__).parent
 logger = logging.getLogger(__name__)
 
 
 OBJECT = Union[str, pydantic.BaseModel, dict]
@@ -39,21 +40,14 @@
 # annotation metamodel
 ANNOTATION_KEY_PROMPT = "prompt"
 ANNOTATION_KEY_PROMPT_SKIP = "prompt.skip"
 ANNOTATION_KEY_ANNOTATORS = "annotators"
 ANNOTATION_KEY_RECURSE = "ner.recurse"
 ANNOTATION_KEY_EXAMPLES = "prompt.examples"
 
-MODEL_GPT_3_5_TURBO = "gpt-3.5-turbo"
-MODEL_TEXT_DAVINCI_003 = "text-davinci-003"
-MODEL_GPT_4 = "gpt-4"
-MODELS = [MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003, MODEL_GPT_4]
-
-DEFAULT_MODEL = MODEL_GPT_3_5_TURBO
-
 # TODO: introspect
 DATAMODELS = [
     "treatment.DiseaseTreatmentSummary",
     "gocam.GoCamAnnotations",
     "bioloigical_process.BiologicalProcess",
     "environmental_sample.Study",
     "mendelian_disease.MendelianDisease",
@@ -99,15 +93,15 @@
     """LinkML SchemaView over the template.
     This is derived from the template and does not need to be set manually."""
 
     api_key: str = None
     """OpenAI API key."""
 
     model: MODEL_NAME = None
-    """OpenAI Model. This should be overridden in subclasses"""
+    """Language Model. This should be overridden in subclasses"""
 
     # annotator: TextAnnotatorInterface = None
     # """Default annotator. TODO: deprecate?"""
 
     annotators: Dict[str, List[TextAnnotatorInterface]] = None
     """Annotators for each class.
     An annotator will ground/map labels to CURIEs.
@@ -152,18 +146,34 @@
     def __post_init__(self):
         if self.template:
             self.template_class = self._get_template_class(self.template)
         if self.template_class:
             logging.info(f"Using template {self.template_class.name}")
         if not self.model:
             self.model = DEFAULT_MODEL
-        self.client = OpenAIClient(model=self.model)
-        logging.info("Setting up OpenAI client API Key")
-        self.api_key = self._get_openai_api_key()
-        openai.api_key = self.api_key
+
+        # Identify model source (e.g., OpenAI)
+        # TODO: move this to its own function
+        all_models = [modelname for model in MODELS for modelname in model]
+        if self.model in all_models:
+            all_openai_models = [modelname for model in OPENAI_MODELS for modelname in model]
+            all_ggml_models = [modelname for model in GGML_MODELS for modelname in model]
+            if self.model in all_openai_models:
+                self.client = OpenAIClient(model=self.model)
+                logging.info("Setting up OpenAI client API Key")
+                self.api_key = self._get_openai_api_key()
+                openai.api_key = self.api_key
+            elif self.model in all_ggml_models:
+                # TODO: optional dependencies here, so catch exception if needed
+                raise NotImplementedError("GPT4ALL models - work in progress")
+        else:
+            raise NotImplementedError(
+                "Model name not recognized or not supported yet."
+                " See all models with `ontogpt list-models`"
+            )
         if self.mappers is None:
             logging.info("Using mappers (currently hardcoded)")
             self.mappers = [get_adapter("translator:")]
         self.encoding = tiktoken.encoding_for_model(self.client.model)
 
     def set_api_key(self, key: str):
         self.api_key = key
```

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.8/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.8/src/ontogpt/engines/spires_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Main Knowledge Extractor class.
 
 This works by recursively constructing structured prompt-completions where
 a pseudo-YAML structure is requested, where the YAML
 structure corresponds to a template class.
 
-Describes in the SPIRES manuscript
+Describe in the SPIRES manuscript
 TODO: add link
 """
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
@@ -34,15 +34,15 @@
 RESPONSE_DICT = Dict[FIELD, Union[RESPONSE_ATOM, List[RESPONSE_ATOM]]]
 
 
 @dataclass
 class SPIRESEngine(KnowledgeEngine):
     """Knowledge extractor."""
 
-    engine: str = "text-davinci-003"
+    engine: str = "openai-text-davinci-003"
     recurse: bool = True
     """If true, then complex non-named entity objects are always recursively parsed.
     If this is false AND the complex object is a pair, then token-based splitting is
     instead used.
     TODO: deprecate this, it's not clear that token-based splitting is better, due to
     the inability to control which tokens GPT will use"""
```

### Comparing `ontogpt-0.2.7/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.8/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.8/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.8/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.8/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/enrichment/eval_enrichment.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/enrichment/eval_enrichment.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,16 @@
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.parsers.association_parser_factory import get_association_parser
 from pydantic import BaseModel
 from tiktoken import Encoding
 
 from ontogpt.engines import create_engine
 from ontogpt.engines.enrichment import ENTITY_ID, EnrichmentEngine, EnrichmentPayload
-from ontogpt.engines.knowledge_engine import (
-    MODEL_GPT_3_5_TURBO,
-    MODEL_GPT_4,
-    MODEL_NAME,
-    MODEL_TEXT_DAVINCI_003,
-)
+from ontogpt.engines.knowledge_engine import MODEL_NAME
+from ontogpt.engines.models import MODEL_GPT_3_5_TURBO, MODEL_GPT_4, MODEL_TEXT_DAVINCI_003
 from ontogpt.evaluation.evaluation_engine import EvaluationEngine
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.utils.gene_set_utils import SYMBOL, GeneSet, drop_genes_from_gene_set, gene_info
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
 
@@ -93,15 +89,16 @@
 
     def __post_init__(self):
         ontology = get_implementation_from_shorthand("sqlite:obo:go")
         if not isinstance(ontology, OboGraphInterface):
             raise TypeError
         self.ontology: ClassEnrichmentCalculationInterface = ontology
         self.engine: EnrichmentEngine = create_engine(None, EnrichmentEngine, model=self.model)
-        for model in ENRICHMENT_MODELS:
+        for modelname in ENRICHMENT_MODELS:
+            model = modelname[0]
             self.engines[model] = create_engine(None, EnrichmentEngine, model=model)
             self.engines[model].add_resolver("sqlite:obo:hgnc")
         self.engine.add_resolver("sqlite:obo:hgnc")
         self.tokenizer_encoding = tiktoken.encoding_for_model(self.engine.model)
 
     def evaluate_methods_on_gene_set(
         self, gene_set: GeneSet, max_size=999, n=4, randomize_gene_descriptions=False, **kwargs
@@ -134,16 +131,16 @@
             comparisons.append(comp)
         return comparisons
 
     def compare_analysis(self, gene_set: GeneSet, **kwargs) -> GeneSetComparison:
         """Compare OntoGPT enrichment vs standard."""
         payloads = {}
         logger.info(f"Gene symbols: {gene_set.gene_symbols}")
-        for model in ENRICHMENT_MODELS:
-            engine = self.engines[model]
+        for modelname in ENRICHMENT_MODELS:
+            engine = self.engines[modelname[0]]
             for method in [NO_SYNOPSIS, ONTOLOGICAL_SYNOPSIS, NARRATIVE_SYNOPSIS]:
                 if method == ONTOLOGICAL_SYNOPSIS:
                     args = dict(ontological_synopsis=True)
                 elif method == NARRATIVE_SYNOPSIS:
                     args = dict(ontological_synopsis=False)
                 elif method == NO_SYNOPSIS:
                     args = dict(annotations=False)
```

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt` & `ontogpt-0.2.8/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml` & `ontogpt-0.2.8/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.8/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.8/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.8/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.8/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.2.8/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2` & `ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2` & `ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2` & `ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2` & `ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2` & `ontogpt-0.2.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/prompts/similarity/connections.jinja2` & `ontogpt-0.2.8/src/ontogpt/prompts/similarity/connections.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/streamlit/spindoctor.py` & `ontogpt-0.2.8/src/ontogpt/streamlit/spindoctor.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 
 openai_api_key = col1.text_input(
     "OpenAI API Key:",
     placeholder="(sk-...) Press [Enter] to submit.",
 )
 
-
 # Button for parsing and displaying the names
 if col1.button("Summarize genes"):
     gene_symbols = [symbol.strip() for symbol in re.split(r"[\-,;\s]+", gene_symbols)]
     gene_set = GeneSet(name="TEMP", gene_symbols=gene_symbols)
     ke = create_engine(None, EnrichmentEngine, model=model)
     if openai_api_key:
         ke.set_api_key(openai_api_key)
```

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.8/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.py` & `ontogpt-0.2.8/src/ontogpt/templates/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/class_enrichment.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/composite_disease.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/composite_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/core.py` & `ontogpt-0.2.8/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/core.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -137,8 +137,8 @@
       UNSPECIFIED_METHOD_OF_ADMINISTRATION:
         meaning: NCIT:C149701
       NOT_APPLICABLE:
         meaning: NCIT:C18902
         aliases:
           - "not applicable"
           - "N/A"
-      NOT_MENTIONED:
+      NOT_MENTIONED:
```

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.8/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.py` & `ontogpt-0.2.8/src/ontogpt/templates/diagnostic_procedure.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/diagnostic_procedure.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/diagnostic_procedure.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/drug.py` & `ontogpt-0.2.8/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.8/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/environmental_sample.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 classes:
   Study:
     tree_root: true
     attributes:
       location:
         description: the sites at which the study was conducted
         annotations:
-          prompt: semicolon-separated list of sites at which the study was conducted
+          prompt: semicolon-separated list of sites at which the study was conducted. give specific place names. if you cannot find a specific place name leave the field as empty.
         range: Location
         multivalued: true
 
       environmental_material:
         description: the environmental material that was sampled
         annotations:
           prompt: semicolon-separated list of environmental materials
         range: EnvironmentalMaterial
         multivalued: true
 
       environments:
         annotations:
-          prompt: semicolon-separated list of environmental contexts in which the study was conducted
+          prompt: semicolon-separated list of environment terms for the location in which the study was conducted
         multivalued: true
         range: Environment
 
       causal_relationships:
         annotations:
           prompt: semicolon-separated list of cause-effect pairs, for example, effect of temperature on growth
         range: CausalRelationship
@@ -58,39 +58,43 @@
         multivalued: true
 
   Location:
     is_a: NamedEntity
     id_prefixes:
       - ENVO
       - GAZ
+      - ENVTHES
     annotations:
-      annotators: sqlite:obo:envo, bioportal:gaz
+      annotators: sqlite:obo:envo, bioportal:gaz, bioportal:envthes
 
   EnvironmentalMaterial:
     is_a: NamedEntity
     id_prefixes:
       - ENVO
+      - ENVTHES
     annotations:
-      annotators: sqlite:obo:envo
+      annotators: sqlite:obo:envo, bioportal:envthes
 
   Environment:
     is_a: NamedEntity
     id_prefixes:
       - ENVO
+      - ENVTHES
     annotations:
-      annotators: sqlite:obo:envo
+      annotators: sqlite:obo:envo, bioportal:envthes
 
   Variable:
     is_a: NamedEntity
     id_prefixes:
       - ENVO
       - MIXS
       - PATO
+      - ENVTHES
     annotations:
-      annotators: sqlite:obo:envo, bioportal:bero
+      annotators: sqlite:obo:envo, bioportal:bero, bioportal:envthes
 
   Unit:
     is_a: NamedEntity
     id_prefixes:
       - UO
       - NCIT
     annotations:
```

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.2.8/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/gene_description_term.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.8/src/ontogpt/templates/gocam.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/halo.py` & `ontogpt-0.2.8/src/ontogpt/templates/halo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ibd.py` & `ontogpt-0.2.8/src/ontogpt/templates/ibd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/ibd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.8/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.8/src/ontogpt/templates/metabolic_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.8/src/ontogpt/templates/metagenome_study.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.8/src/ontogpt/templates/ontology_class.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.py` & `ontogpt-0.2.8/src/ontogpt/templates/ontology_issue.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/ontology_issue.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/ontology_issue.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.8/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.8/src/ontogpt/templates/reaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.8/src/ontogpt/templates/recipe.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/traits.py` & `ontogpt-0.2.8/src/ontogpt/templates/biotic_interaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,25 +24,25 @@
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     NOT_APPLICABLE = "NOT_APPLICABLE"
     NOT_MENTIONED = "NOT_MENTIONED"
     
     
 
-class Taxon(ConfiguredBaseModel):
+class Container(ConfiguredBaseModel):
     
-    metabolic_traits: Optional[List[str]] = Field(default_factory=list, description="""The metabolic traits for the taxon.""")
-    morphological_traits: Optional[List[str]] = Field(default_factory=list, description="""The morphological traits for the taxon.""")
-    genetic_traits: Optional[List[str]] = Field(default_factory=list, description="""The genetic traits for the taxon.""")
-    cellular_traits: Optional[List[str]] = Field(default_factory=list, description="""The cellular traits for the taxon.""")
-    ecological_traits: Optional[List[str]] = Field(default_factory=list, description="""The ecological traits for the taxon.""")
-    reproductive_traits: Optional[List[str]] = Field(default_factory=list, description="""The reproductive traits for the taxon.""")
-    survival_traits: Optional[List[str]] = Field(default_factory=list, description="""The survival traits for the taxon.""")
-    phenotypic_plasticiticy_traits: Optional[List[str]] = Field(default_factory=list, description="""The phenotypic plasticiticy traits for the taxon.""")
-    preferred_environments: Optional[List[str]] = Field(default_factory=list, description="""The preferred environments for the taxon.""")
+    interactions: Optional[List[BioticInteraction]] = Field(default_factory=list)
+    
+
+
+class BioticInteraction(ConfiguredBaseModel):
+    
+    source_taxon: Optional[str] = Field(None, description="""the taxon that is the subject of the interaction""")
+    target_taxon: Optional[str] = Field(None, description="""the taxon that is the object of the ineteraction""")
+    interaction_type: Optional[str] = Field(None, description="""the type of interaction""")
     
 
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
@@ -59,15 +59,22 @@
 class NamedEntity(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
 
 
-class Trait(NamedEntity):
+class Taxon(NamedEntity):
+    
+    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
+    
+
+
+class InteractionType(NamedEntity):
     
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
 
 
 class CompoundExpression(ConfiguredBaseModel):
@@ -120,18 +127,20 @@
     object_text: Optional[str] = Field(None)
     
 
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
-Taxon.update_forward_refs()
+Container.update_forward_refs()
+BioticInteraction.update_forward_refs()
 ExtractionResult.update_forward_refs()
 NamedEntity.update_forward_refs()
-Trait.update_forward_refs()
+Taxon.update_forward_refs()
+InteractionType.update_forward_refs()
 CompoundExpression.update_forward_refs()
 Triple.update_forward_refs()
 TextWithTriples.update_forward_refs()
 RelationshipType.update_forward_refs()
 Publication.update_forward_refs()
 AnnotatorResult.update_forward_refs()
```

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/traits.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/traits.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.8/src/ontogpt/templates/treatment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.8/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/utils/gene_set_utils.py` & `ontogpt-0.2.8/src/ontogpt/utils/gene_set_utils.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.8/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.2.8/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.7/src/ontogpt/webapp/main.py` & `ontogpt-0.2.8/src/ontogpt/webapp/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import uvicorn
 from fastapi import FastAPI, Form, Request
 from pydantic import BaseModel
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
 
 from ontogpt.engines.enrichment import EnrichmentEngine
-from ontogpt.engines.knowledge_engine import DATAMODELS, MODELS
+from ontogpt.engines.knowledge_engine import DATAMODELS
+from ontogpt.engines.models import MODELS
 from ontogpt.engines.spires_engine import SPIRESEngine
 from ontogpt.io.html_exporter import HTMLExporter
 from ontogpt.utils.gene_set_utils import GeneSet
 
 this_path = Path(__file__).parent
 static_dir = this_path / "static"
 html_dir = this_path / "html"
@@ -59,16 +60,17 @@
     return templates.TemplateResponse(
         "results.html", context={"request": request, "inner_html": output.getvalue()}
     )
 
 
 @app.get("/spindoctor")
 def sd_read_root(request: Request):
+    all_models = [modelname for model in MODELS for modelname in model]
     return templates.TemplateResponse(
-        "spindoctor/form.html", context={"request": request, "models": MODELS}
+        "spindoctor/form.html", context={"request": request, "models": all_models}
     )
 
 
 @app.post("/spindoctor")
 def sd_form_post(request: Request, model: str = Form(...), text: str = Form(...)):
     print(f"Received request with model {model}")
     print(f"Received request with text {text}")
```

### Comparing `ontogpt-0.2.7/PKG-INFO` & `ontogpt-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.7
+Version: 0.2.8
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+Provides-Extra: gpt4all
 Provides-Extra: recipes
+Provides-Extra: textract
 Provides-Extra: web
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) ; extra == "web"
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0,!=1.4.46)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: bioc (>=2.0.post5,<3.0)
 Requires-Dist: cachier (>=2.1.0,<3.0.0)
-Requires-Dist: class-resolver
+Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: eutils (>=0.6.0,<0.7.0)
 Requires-Dist: fastapi (>=0.88.0,<0.89.0) ; extra == "web"
 Requires-Dist: gilda (>=0.10.3,<0.11.0)
 Requires-Dist: gpt4 (>=0.0.1,<0.0.2)
 Requires-Dist: greenlet (!=2.0.2)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: inflect (>=6.0.2,<7.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
+Requires-Dist: langchain (>=0.0.167,<0.0.168)
 Requires-Dist: linkml (>=1.4.10,<2.0.0)
 Requires-Dist: linkml-owl (>=0.2.7,<0.3.0)
-Requires-Dist: linkml-runtime (>=1.4.9,<2.0.0)
+Requires-Dist: linkml-runtime (>=1.5.3,<2.0.0)
 Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: nlpcloud (>=1.0.39,<2.0.0)
 Requires-Dist: oaklib (>=0.5.6,<0.6.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
+Requires-Dist: pygpt4all[gpt4all] (>=1.1.0,<2.0.0) ; extra == "gpt4all"
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: recipe-scrapers[recipes] (>=14.35.0,<15.0.0) ; extra == "recipes"
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: rustsim (>=0.1.8,<0.2.0)
+Requires-Dist: semsimian (>=0.1.13)
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: streamlit (>=1.22.0,<2.0.0)
+Requires-Dist: textract[textract] ; extra == "textract"
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "web"
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Requires-Dist: wikipedia-api (>=0.5.8,<0.6.0)
 Description-Content-Type: text/markdown
 
 # OntoGPT
```

