# Comparing `tmp/semantha_sdk-5.3.0.tar.gz` & `tmp/semantha_sdk-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.3.0.tar", max compression
+gzip compressed data, was "semantha_sdk-5.3.1.tar", max compression
```

## Comparing `semantha_sdk-5.3.0.tar` & `semantha_sdk-5.3.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.3.0/LICENSE
--rw-r--r--   0        0        0     1618 2023-06-01 10:22:16.570565 semantha_sdk-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     7795 2023-06-01 10:21:34.644458 semantha_sdk-5.3.0/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.3.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.3.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1634 2023-06-01 08:29:07.930000 semantha_sdk-5.3.0/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0      930 2023-06-01 08:29:07.488000 semantha_sdk-5.3.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      729 2023-06-01 08:29:07.509000 semantha_sdk-5.3.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      739 2023-06-01 08:29:07.718000 semantha_sdk-5.3.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1628 2023-06-01 08:29:07.588000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1493 2023-06-01 08:29:07.539000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3671 2023-06-01 08:29:07.677000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3423 2023-06-01 08:29:07.710000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1191 2023-06-01 08:29:07.755000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      832 2023-06-01 08:29:07.775000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1730 2023-06-01 08:29:07.765000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1577 2023-06-01 08:29:07.793000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2722 2023-06-01 08:29:07.744000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      726 2023-06-01 08:29:07.726000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1509 2023-06-01 08:29:07.801000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1508 2023-06-01 08:29:07.820000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1216 2023-06-01 08:29:07.830000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1111 2023-06-01 08:29:07.837000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1170 2023-06-01 08:29:07.846000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0      976 2023-06-01 08:29:07.785000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     5667 2023-06-01 08:29:08.061000 semantha_sdk-5.3.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1050 2023-06-01 08:29:07.857000 semantha_sdk-5.3.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1369 2023-06-01 08:29:07.881000 semantha_sdk-5.3.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     2315 2023-06-01 08:29:07.950000 semantha_sdk-5.3.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1387 2023-06-01 08:29:07.972000 semantha_sdk-5.3.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1823 2023-06-01 08:29:07.960000 semantha_sdk-5.3.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3566 2023-06-01 08:29:07.990000 semantha_sdk-5.3.0/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     3497 2023-06-01 08:29:08.005000 semantha_sdk-5.3.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     4161 2023-06-01 08:29:07.915000 semantha_sdk-5.3.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1013 2023-06-01 08:29:07.890000 semantha_sdk-5.3.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      791 2023-06-01 08:29:08.258000 semantha_sdk-5.3.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1648 2023-06-01 08:29:08.270000 semantha_sdk-5.3.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1529 2023-06-01 08:29:08.280000 semantha_sdk-5.3.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1545 2023-06-01 08:29:08.333000 semantha_sdk-5.3.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0      762 2023-06-01 08:29:08.287000 semantha_sdk-5.3.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     1524 2023-06-01 08:29:08.309000 semantha_sdk-5.3.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      706 2023-06-01 08:29:08.299000 semantha_sdk-5.3.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0      777 2023-06-01 08:29:08.359000 semantha_sdk-5.3.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      774 2023-06-01 08:29:08.365000 semantha_sdk-5.3.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1514 2023-06-01 08:29:08.351000 semantha_sdk-5.3.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1107 2023-06-01 08:29:08.014000 semantha_sdk-5.3.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     2315 2023-06-01 08:29:08.024000 semantha_sdk-5.3.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1546 2023-06-01 08:29:08.068000 semantha_sdk-5.3.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1494 2023-06-01 08:29:08.108000 semantha_sdk-5.3.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      682 2023-06-01 08:29:08.100000 semantha_sdk-5.3.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0    14477 2023-05-11 17:26:57.378270 semantha_sdk-5.3.0/semantha_sdk/api/reference_documents.py
--rw-r--r--   0        0        0     2074 2023-06-01 08:29:08.094000 semantha_sdk-5.3.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0     8930 2023-06-01 08:29:08.047000 semantha_sdk-5.3.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0     6565 2023-06-01 08:29:08.149000 semantha_sdk-5.3.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      789 2023-06-01 08:29:07.866000 semantha_sdk-5.3.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.3.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.3.0/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      836 2023-06-01 08:29:08.122000 semantha_sdk-5.3.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      676 2023-06-01 08:29:08.114000 semantha_sdk-5.3.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1379 2023-06-01 08:29:08.158000 semantha_sdk-5.3.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5389 2023-06-01 08:29:08.174000 semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     4015 2023-06-01 08:29:08.199000 semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      844 2023-06-01 08:29:08.077000 semantha_sdk-5.3.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0      840 2023-06-01 08:29:08.220000 semantha_sdk-5.3.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1115 2023-06-01 08:29:08.230000 semantha_sdk-5.3.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0      912 2023-06-01 08:29:08.210000 semantha_sdk-5.3.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1310 2023-06-01 08:29:08.248000 semantha_sdk-5.3.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     4241 2023-06-01 08:29:09.369000 semantha_sdk-5.3.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      607 2023-06-01 08:29:08.744000 semantha_sdk-5.3.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      654 2023-06-01 08:29:08.982000 semantha_sdk-5.3.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      556 2023-06-01 08:29:08.895000 semantha_sdk-5.3.0/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      535 2023-06-01 08:29:09.185000 semantha_sdk-5.3.0/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      546 2023-06-01 08:29:08.875000 semantha_sdk-5.3.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      930 2023-06-01 08:29:08.889000 semantha_sdk-5.3.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      508 2023-06-01 08:29:08.779000 semantha_sdk-5.3.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      672 2023-06-01 08:29:08.964000 semantha_sdk-5.3.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0     1139 2023-06-01 08:29:08.852000 semantha_sdk-5.3.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      516 2023-06-01 08:29:09.034000 semantha_sdk-5.3.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      604 2023-06-01 08:29:09.256000 semantha_sdk-5.3.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      476 2023-06-01 08:29:09.024000 semantha_sdk-5.3.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      519 2023-06-01 08:29:09.003000 semantha_sdk-5.3.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1213 2023-06-01 08:29:09.247000 semantha_sdk-5.3.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0      939 2023-06-01 08:29:09.159000 semantha_sdk-5.3.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      723 2023-06-01 08:29:09.098000 semantha_sdk-5.3.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      566 2023-06-01 08:29:08.773000 semantha_sdk-5.3.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      628 2023-06-01 08:29:08.971000 semantha_sdk-5.3.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1004 2023-06-01 08:29:09.123000 semantha_sdk-5.3.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      503 2023-06-01 08:29:09.011000 semantha_sdk-5.3.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      498 2023-06-01 08:29:08.737000 semantha_sdk-5.3.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      564 2023-06-01 08:29:08.701000 semantha_sdk-5.3.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      447 2023-06-01 08:29:09.107000 semantha_sdk-5.3.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      597 2023-06-01 08:29:08.795000 semantha_sdk-5.3.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      729 2023-06-01 08:29:08.991000 semantha_sdk-5.3.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      536 2023-06-01 08:29:09.029000 semantha_sdk-5.3.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      842 2023-06-01 08:29:08.946000 semantha_sdk-5.3.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      512 2023-06-01 08:29:08.997000 semantha_sdk-5.3.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      498 2023-06-01 08:29:08.921000 semantha_sdk-5.3.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      524 2023-06-01 08:29:08.956000 semantha_sdk-5.3.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      839 2023-06-01 08:29:09.071000 semantha_sdk-5.3.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      531 2023-06-01 08:29:08.732000 semantha_sdk-5.3.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      408 2023-06-01 08:29:08.878000 semantha_sdk-5.3.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      474 2023-06-01 08:29:08.924000 semantha_sdk-5.3.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      576 2023-06-01 08:29:08.840000 semantha_sdk-5.3.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      483 2023-06-01 08:29:08.784000 semantha_sdk-5.3.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      582 2023-06-01 08:29:08.692000 semantha_sdk-5.3.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      499 2023-06-01 08:29:08.809000 semantha_sdk-5.3.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      493 2023-06-01 08:29:08.708000 semantha_sdk-5.3.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      430 2023-06-01 08:29:08.632000 semantha_sdk-5.3.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      528 2023-06-01 08:29:08.915000 semantha_sdk-5.3.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1482 2023-06-01 08:29:08.761000 semantha_sdk-5.3.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      485 2023-06-01 08:29:08.901000 semantha_sdk-5.3.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      787 2023-06-01 08:29:08.908000 semantha_sdk-5.3.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      528 2023-06-01 08:29:08.868000 semantha_sdk-5.3.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0      948 2023-06-01 08:29:09.134000 semantha_sdk-5.3.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      486 2023-06-01 08:29:09.102000 semantha_sdk-5.3.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      493 2023-06-01 08:29:09.138000 semantha_sdk-5.3.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      577 2023-06-01 08:29:08.802000 semantha_sdk-5.3.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      445 2023-06-01 08:29:09.018000 semantha_sdk-5.3.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      775 2023-06-01 08:29:09.050000 semantha_sdk-5.3.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      728 2023-06-01 08:29:08.626000 semantha_sdk-5.3.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      646 2023-06-01 08:29:09.218000 semantha_sdk-5.3.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.3.0/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      873 2023-06-01 08:29:09.086000 semantha_sdk-5.3.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      518 2023-06-01 08:29:08.814000 semantha_sdk-5.3.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      792 2023-06-01 08:29:08.864000 semantha_sdk-5.3.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1669 2023-06-01 08:29:08.834000 semantha_sdk-5.3.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      454 2023-06-01 08:29:08.932000 semantha_sdk-5.3.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      695 2023-06-01 08:29:09.038000 semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      851 2023-06-01 08:29:08.724000 semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      608 2023-06-01 08:29:08.669000 semantha_sdk-5.3.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      480 2023-06-01 08:29:08.788000 semantha_sdk-5.3.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      542 2023-06-01 08:29:08.647000 semantha_sdk-5.3.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      466 2023-06-01 08:29:08.715000 semantha_sdk-5.3.0/semantha_sdk/model/table.py
--rw-r--r--   0        0        0      565 2023-06-01 08:29:09.165000 semantha_sdk-5.3.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      462 2023-06-01 08:29:08.750000 semantha_sdk-5.3.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      464 2023-06-01 08:29:08.680000 semantha_sdk-5.3.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.3.0/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.3.0/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.3.0/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.3.0/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.3.0/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.3.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.3.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0     8464 1970-01-01 00:00:00.000000 semantha_sdk-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.3.1/LICENSE
+-rw-r--r--   0        0        0     1618 2023-06-01 13:11:28.778568 semantha_sdk-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7795 2023-06-01 10:21:34.644458 semantha_sdk-5.3.1/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.3.1/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.3.1/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1634 2023-06-01 08:29:07.930000 semantha_sdk-5.3.1/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0      930 2023-06-01 08:29:07.488000 semantha_sdk-5.3.1/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      729 2023-06-01 08:29:07.509000 semantha_sdk-5.3.1/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      739 2023-06-01 08:29:07.718000 semantha_sdk-5.3.1/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1628 2023-06-01 08:29:07.588000 semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1493 2023-06-01 08:29:07.539000 semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3671 2023-06-01 08:29:07.677000 semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3423 2023-06-01 08:29:07.710000 semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1191 2023-06-01 08:29:07.755000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      832 2023-06-01 08:29:07.775000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1730 2023-06-01 08:29:07.765000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1577 2023-06-01 08:29:07.793000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2722 2023-06-01 08:29:07.744000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      726 2023-06-01 08:29:07.726000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1509 2023-06-01 08:29:07.801000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1508 2023-06-01 08:29:07.820000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1216 2023-06-01 08:29:07.830000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1111 2023-06-01 08:29:07.837000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1170 2023-06-01 08:29:07.846000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0      976 2023-06-01 08:29:07.785000 semantha_sdk-5.3.1/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     5667 2023-06-01 08:29:08.061000 semantha_sdk-5.3.1/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1050 2023-06-01 08:29:07.857000 semantha_sdk-5.3.1/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1369 2023-06-01 08:29:07.881000 semantha_sdk-5.3.1/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     2315 2023-06-01 08:29:07.950000 semantha_sdk-5.3.1/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1387 2023-06-01 08:29:07.972000 semantha_sdk-5.3.1/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1823 2023-06-01 08:29:07.960000 semantha_sdk-5.3.1/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3566 2023-06-01 08:29:07.990000 semantha_sdk-5.3.1/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     3497 2023-06-01 08:29:08.005000 semantha_sdk-5.3.1/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     4161 2023-06-01 08:29:07.915000 semantha_sdk-5.3.1/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1013 2023-06-01 08:29:07.890000 semantha_sdk-5.3.1/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      791 2023-06-01 08:29:08.258000 semantha_sdk-5.3.1/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1648 2023-06-01 08:29:08.270000 semantha_sdk-5.3.1/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1529 2023-06-01 08:29:08.280000 semantha_sdk-5.3.1/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1545 2023-06-01 08:29:08.333000 semantha_sdk-5.3.1/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0      762 2023-06-01 08:29:08.287000 semantha_sdk-5.3.1/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     1524 2023-06-01 08:29:08.309000 semantha_sdk-5.3.1/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      706 2023-06-01 08:29:08.299000 semantha_sdk-5.3.1/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0      777 2023-06-01 08:29:08.359000 semantha_sdk-5.3.1/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      774 2023-06-01 08:29:08.365000 semantha_sdk-5.3.1/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1514 2023-06-01 08:29:08.351000 semantha_sdk-5.3.1/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1107 2023-06-01 08:29:08.014000 semantha_sdk-5.3.1/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     2315 2023-06-01 08:29:08.024000 semantha_sdk-5.3.1/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1546 2023-06-01 08:29:08.068000 semantha_sdk-5.3.1/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1494 2023-06-01 08:29:08.108000 semantha_sdk-5.3.1/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      682 2023-06-01 08:29:08.100000 semantha_sdk-5.3.1/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0    14477 2023-05-11 17:26:57.378270 semantha_sdk-5.3.1/semantha_sdk/api/reference_documents.py
+-rw-r--r--   0        0        0     2074 2023-06-01 08:29:08.094000 semantha_sdk-5.3.1/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0     8930 2023-06-01 08:29:08.047000 semantha_sdk-5.3.1/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0     6565 2023-06-01 08:29:08.149000 semantha_sdk-5.3.1/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      789 2023-06-01 08:29:07.866000 semantha_sdk-5.3.1/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.3.1/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.3.1/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      836 2023-06-01 08:29:08.122000 semantha_sdk-5.3.1/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      676 2023-06-01 08:29:08.114000 semantha_sdk-5.3.1/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1379 2023-06-01 08:29:08.158000 semantha_sdk-5.3.1/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5389 2023-06-01 08:29:08.174000 semantha_sdk-5.3.1/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4015 2023-06-01 08:29:08.199000 semantha_sdk-5.3.1/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      844 2023-06-01 08:29:08.077000 semantha_sdk-5.3.1/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0      840 2023-06-01 08:29:08.220000 semantha_sdk-5.3.1/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1115 2023-06-01 08:29:08.230000 semantha_sdk-5.3.1/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0      912 2023-06-01 08:29:08.210000 semantha_sdk-5.3.1/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1310 2023-06-01 08:29:08.248000 semantha_sdk-5.3.1/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     4241 2023-06-01 08:29:09.369000 semantha_sdk-5.3.1/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-01 08:29:08.744000 semantha_sdk-5.3.1/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      654 2023-06-01 08:29:08.982000 semantha_sdk-5.3.1/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      556 2023-06-01 08:29:08.895000 semantha_sdk-5.3.1/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      535 2023-06-01 08:29:09.185000 semantha_sdk-5.3.1/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      546 2023-06-01 08:29:08.875000 semantha_sdk-5.3.1/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      930 2023-06-01 08:29:08.889000 semantha_sdk-5.3.1/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      508 2023-06-01 08:29:08.779000 semantha_sdk-5.3.1/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      672 2023-06-01 08:29:08.964000 semantha_sdk-5.3.1/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0     1139 2023-06-01 08:29:08.852000 semantha_sdk-5.3.1/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      516 2023-06-01 08:29:09.034000 semantha_sdk-5.3.1/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      604 2023-06-01 08:29:09.256000 semantha_sdk-5.3.1/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      476 2023-06-01 08:29:09.024000 semantha_sdk-5.3.1/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      519 2023-06-01 08:29:09.003000 semantha_sdk-5.3.1/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1213 2023-06-01 08:29:09.247000 semantha_sdk-5.3.1/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0      939 2023-06-01 08:29:09.159000 semantha_sdk-5.3.1/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      723 2023-06-01 08:29:09.098000 semantha_sdk-5.3.1/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      566 2023-06-01 08:29:08.773000 semantha_sdk-5.3.1/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      628 2023-06-01 08:29:08.971000 semantha_sdk-5.3.1/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1004 2023-06-01 08:29:09.123000 semantha_sdk-5.3.1/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      503 2023-06-01 08:29:09.011000 semantha_sdk-5.3.1/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      498 2023-06-01 08:29:08.737000 semantha_sdk-5.3.1/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      564 2023-06-01 08:29:08.701000 semantha_sdk-5.3.1/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      447 2023-06-01 08:29:09.107000 semantha_sdk-5.3.1/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      597 2023-06-01 08:29:08.795000 semantha_sdk-5.3.1/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      729 2023-06-01 08:29:08.991000 semantha_sdk-5.3.1/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      536 2023-06-01 08:29:09.029000 semantha_sdk-5.3.1/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      842 2023-06-01 08:29:08.946000 semantha_sdk-5.3.1/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      512 2023-06-01 08:29:08.997000 semantha_sdk-5.3.1/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      498 2023-06-01 08:29:08.921000 semantha_sdk-5.3.1/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      524 2023-06-01 08:29:08.956000 semantha_sdk-5.3.1/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      839 2023-06-01 08:29:09.071000 semantha_sdk-5.3.1/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      531 2023-06-01 08:29:08.732000 semantha_sdk-5.3.1/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      408 2023-06-01 08:29:08.878000 semantha_sdk-5.3.1/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      474 2023-06-01 08:29:08.924000 semantha_sdk-5.3.1/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      576 2023-06-01 08:29:08.840000 semantha_sdk-5.3.1/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      483 2023-06-01 08:29:08.784000 semantha_sdk-5.3.1/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      582 2023-06-01 08:29:08.692000 semantha_sdk-5.3.1/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      499 2023-06-01 08:29:08.809000 semantha_sdk-5.3.1/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      493 2023-06-01 08:29:08.708000 semantha_sdk-5.3.1/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      430 2023-06-01 08:29:08.632000 semantha_sdk-5.3.1/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      528 2023-06-01 08:29:08.915000 semantha_sdk-5.3.1/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1482 2023-06-01 08:29:08.761000 semantha_sdk-5.3.1/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      485 2023-06-01 08:29:08.901000 semantha_sdk-5.3.1/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      787 2023-06-01 08:29:08.908000 semantha_sdk-5.3.1/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      528 2023-06-01 08:29:08.868000 semantha_sdk-5.3.1/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0      948 2023-06-01 08:29:09.134000 semantha_sdk-5.3.1/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      486 2023-06-01 08:29:09.102000 semantha_sdk-5.3.1/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      493 2023-06-01 08:29:09.138000 semantha_sdk-5.3.1/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      577 2023-06-01 08:29:08.802000 semantha_sdk-5.3.1/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      445 2023-06-01 08:29:09.018000 semantha_sdk-5.3.1/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      775 2023-06-01 08:29:09.050000 semantha_sdk-5.3.1/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      728 2023-06-01 08:29:08.626000 semantha_sdk-5.3.1/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      646 2023-06-01 08:29:09.218000 semantha_sdk-5.3.1/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.3.1/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      873 2023-06-01 08:29:09.086000 semantha_sdk-5.3.1/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      518 2023-06-01 08:29:08.814000 semantha_sdk-5.3.1/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      792 2023-06-01 08:29:08.864000 semantha_sdk-5.3.1/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1669 2023-06-01 08:29:08.834000 semantha_sdk-5.3.1/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      454 2023-06-01 08:29:08.932000 semantha_sdk-5.3.1/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      695 2023-06-01 08:29:09.038000 semantha_sdk-5.3.1/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      851 2023-06-01 08:29:08.724000 semantha_sdk-5.3.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      608 2023-06-01 08:29:08.669000 semantha_sdk-5.3.1/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      480 2023-06-01 08:29:08.788000 semantha_sdk-5.3.1/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      542 2023-06-01 08:29:08.647000 semantha_sdk-5.3.1/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      476 2023-06-01 13:10:58.286104 semantha_sdk-5.3.1/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      565 2023-06-01 08:29:09.165000 semantha_sdk-5.3.1/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      462 2023-06-01 08:29:08.750000 semantha_sdk-5.3.1/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      464 2023-06-01 08:29:08.680000 semantha_sdk-5.3.1/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.3.1/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.3.1/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.3.1/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.3.1/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.3.1/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.3.1/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.3.1/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0     8464 1970-01-01 00:00:00.000000 semantha_sdk-5.3.1/PKG-INFO
```

### Comparing `semantha_sdk-5.3.0/LICENSE` & `semantha_sdk-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/pyproject.toml` & `semantha_sdk-5.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.3.0"
+version = "5.3.1"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-5.3.0/README.md` & `semantha_sdk-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/__init__.py` & `semantha_sdk-5.3.1/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/answers.py` & `semantha_sdk-5.3.1/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulk.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.3.1/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/clusters.py` & `semantha_sdk-5.3.1/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.3.1/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/diff.py` & `semantha_sdk-5.3.1/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.3.1/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.3.1/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.3.1/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.3.1/semantha_sdk/api/documentcomparisons.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/documents.py` & `semantha_sdk-5.3.1/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/domain.py` & `semantha_sdk-5.3.1/semantha_sdk/api/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/domains.py` & `semantha_sdk-5.3.1/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/info.py` & `semantha_sdk-5.3.1/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/languages.py` & `semantha_sdk-5.3.1/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.3.1/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.3.1/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.3.1/semantha_sdk/api/modelinstances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.3.1/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.3.1/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.3.1/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/reference_documents.py` & `semantha_sdk-5.3.1/semantha_sdk/api/reference_documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.3.1/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.3.1/semantha_sdk/api/referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/references.py` & `semantha_sdk-5.3.1/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/roles.py` & `semantha_sdk-5.3.1/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.3.1/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/sentence.py` & `semantha_sdk-5.3.1/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/sentences.py` & `semantha_sdk-5.3.1/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/settings.py` & `semantha_sdk-5.3.1/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.3.1/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.3.1/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/statistic.py` & `semantha_sdk-5.3.1/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/tag.py` & `semantha_sdk-5.3.1/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.3.1/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/tags.py` & `semantha_sdk-5.3.1/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/api/validation.py` & `semantha_sdk-5.3.1/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/__init__.py` & `semantha_sdk-5.3.1/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.3.1/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.3.1/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/answer.py` & `semantha_sdk-5.3.1/semantha_sdk/model/answer.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.3.1/semantha_sdk/model/answer_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.3.1/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.3.1/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.3.1/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.3.1/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/current_user.py` & `semantha_sdk-5.3.1/semantha_sdk/model/current_user.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/data_property.py` & `semantha_sdk-5.3.1/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/distance.py` & `semantha_sdk-5.3.1/semantha_sdk/model/distance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/document.py` & `semantha_sdk-5.3.1/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/document_class.py` & `semantha_sdk-5.3.1/semantha_sdk/model/document_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.3.1/semantha_sdk/model/document_class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.3.1/semantha_sdk/model/document_class_node.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.3.1/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/document_information.py` & `semantha_sdk-5.3.1/semantha_sdk/model/document_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/domain.py` & `semantha_sdk-5.3.1/semantha_sdk/model/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.3.1/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.3.1/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.3.1/semantha_sdk/model/extraction_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/features.py` & `semantha_sdk-5.3.1/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.3.1/semantha_sdk/model/file_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/info.py` & `semantha_sdk-5.3.1/semantha_sdk/model/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/instance.py` & `semantha_sdk-5.3.1/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.3.1/semantha_sdk/model/instance_child.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.3.1/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.3.1/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/model_class.py` & `semantha_sdk-5.3.1/semantha_sdk/model/model_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.3.1/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/page.py` & `semantha_sdk-5.3.1/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/page_content.py` & `semantha_sdk-5.3.1/semantha_sdk/model/page_content.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.3.1/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/process_information.py` & `semantha_sdk-5.3.1/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/reference.py` & `semantha_sdk-5.3.1/semantha_sdk/model/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.3.1/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-5.3.1/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.3.1/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.3.1/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.3.1/semantha_sdk/model/semi_super_vised_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/sentence.py` & `semantha_sdk-5.3.1/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/settings.py` & `semantha_sdk-5.3.1/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.3.1/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.3.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/statistic.py` & `semantha_sdk-5.3.1/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/synonym.py` & `semantha_sdk-5.3.1/semantha_sdk/model/synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.3.1/semantha_sdk/model/table_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.3.1/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.3.1/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.3.1/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.0/PKG-INFO` & `semantha_sdk-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 5.3.0
+Version: 5.3.1
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
```

