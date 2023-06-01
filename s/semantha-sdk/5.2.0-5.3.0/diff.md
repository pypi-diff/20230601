# Comparing `tmp/semantha_sdk-5.2.0.tar.gz` & `tmp/semantha_sdk-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.2.0.tar", max compression
+gzip compressed data, was "semantha_sdk-5.3.0.tar", max compression
```

## Comparing `semantha_sdk-5.2.0.tar` & `semantha_sdk-5.3.0.tar`

### file list

```diff
@@ -1,142 +1,144 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.2.0/LICENSE
--rw-r--r--   0        0        0     1631 2023-05-22 16:40:37.048488 semantha_sdk-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     7644 2023-05-22 17:43:51.933450 semantha_sdk-5.2.0/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.2.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.2.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0      930 2023-05-22 16:30:13.775000 semantha_sdk-5.2.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      729 2023-05-22 16:30:13.778000 semantha_sdk-5.2.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      739 2023-05-22 16:30:13.812000 semantha_sdk-5.2.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1628 2023-05-22 16:30:13.794000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1493 2023-05-22 16:30:13.784000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3671 2023-05-22 16:30:13.807000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3423 2023-05-22 16:30:13.811000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1191 2023-05-22 16:30:13.818000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      832 2023-05-22 16:30:13.821000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1730 2023-05-22 16:30:13.819000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1577 2023-05-22 16:30:13.825000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2722 2023-05-22 16:30:13.816000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      726 2023-05-22 16:30:13.814000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1509 2023-05-22 16:30:13.827000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1508 2023-05-22 16:30:13.831000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1216 2023-05-22 16:30:13.832000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1111 2023-05-22 16:30:13.834000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1170 2023-05-22 16:30:13.836000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0      976 2023-05-22 16:30:13.823000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     5667 2023-05-22 16:30:13.873000 semantha_sdk-5.2.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1050 2023-05-22 16:30:13.837000 semantha_sdk-5.2.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1369 2023-05-22 16:30:13.840000 semantha_sdk-5.2.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     2315 2023-05-22 16:30:13.848000 semantha_sdk-5.2.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1387 2023-05-22 16:30:13.854000 semantha_sdk-5.2.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1823 2023-05-22 16:30:13.850000 semantha_sdk-5.2.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3566 2023-05-22 16:30:13.857000 semantha_sdk-5.2.0/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     3497 2023-05-22 16:30:13.861000 semantha_sdk-5.2.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     3947 2023-05-22 16:30:13.844000 semantha_sdk-5.2.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1013 2023-05-22 16:30:13.841000 semantha_sdk-5.2.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      791 2023-05-22 16:30:13.906000 semantha_sdk-5.2.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1648 2023-05-22 16:30:13.907000 semantha_sdk-5.2.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1529 2023-05-22 16:30:13.909000 semantha_sdk-5.2.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1545 2023-05-22 16:30:13.914000 semantha_sdk-5.2.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0      762 2023-05-22 16:30:13.910000 semantha_sdk-5.2.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     1524 2023-05-22 16:30:13.913000 semantha_sdk-5.2.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      706 2023-05-22 16:30:13.911000 semantha_sdk-5.2.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0      777 2023-05-22 16:30:13.917000 semantha_sdk-5.2.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      774 2023-05-22 16:30:13.918000 semantha_sdk-5.2.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1514 2023-05-22 16:30:13.916000 semantha_sdk-5.2.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1107 2023-05-22 16:30:13.862000 semantha_sdk-5.2.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     2112 2023-05-22 16:30:13.864000 semantha_sdk-5.2.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1546 2023-05-22 16:30:13.874000 semantha_sdk-5.2.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1494 2023-05-22 16:30:13.881000 semantha_sdk-5.2.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      682 2023-05-22 16:30:13.880000 semantha_sdk-5.2.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0    14477 2023-05-11 17:26:57.378270 semantha_sdk-5.2.0/semantha_sdk/api/reference_documents.py
--rw-r--r--   0        0        0     2074 2023-05-22 16:30:13.878000 semantha_sdk-5.2.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0     8930 2023-05-22 16:30:13.870000 semantha_sdk-5.2.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0     6565 2023-05-22 16:30:13.887000 semantha_sdk-5.2.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      789 2023-05-22 16:30:13.838000 semantha_sdk-5.2.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.2.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.2.0/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      836 2023-05-22 16:30:13.883000 semantha_sdk-5.2.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      676 2023-05-22 16:30:13.882000 semantha_sdk-5.2.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1379 2023-05-22 16:30:13.889000 semantha_sdk-5.2.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5389 2023-05-22 16:30:13.893000 semantha_sdk-5.2.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     4015 2023-05-22 16:30:13.895000 semantha_sdk-5.2.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      844 2023-05-22 16:30:13.875000 semantha_sdk-5.2.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0      840 2023-05-22 16:30:13.899000 semantha_sdk-5.2.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1115 2023-05-22 16:30:13.900000 semantha_sdk-5.2.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0      912 2023-05-22 16:30:13.897000 semantha_sdk-5.2.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1310 2023-05-22 16:30:13.905000 semantha_sdk-5.2.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     4129 2023-05-22 16:30:14.061000 semantha_sdk-5.2.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      607 2023-05-22 16:30:14.008000 semantha_sdk-5.2.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      654 2023-05-22 16:30:14.026000 semantha_sdk-5.2.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      546 2023-05-22 16:30:13.977000 semantha_sdk-5.2.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      930 2023-05-22 16:30:13.985000 semantha_sdk-5.2.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      508 2023-05-22 16:30:14.043000 semantha_sdk-5.2.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      672 2023-05-22 16:30:14.005000 semantha_sdk-5.2.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0     1139 2023-05-22 16:30:14.045000 semantha_sdk-5.2.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      516 2023-05-22 16:30:14.034000 semantha_sdk-5.2.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      604 2023-05-22 16:30:13.967000 semantha_sdk-5.2.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      476 2023-05-22 16:30:13.978000 semantha_sdk-5.2.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      519 2023-05-22 16:30:14.047000 semantha_sdk-5.2.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1213 2023-05-22 16:30:14.002000 semantha_sdk-5.2.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0      939 2023-05-22 16:30:13.988000 semantha_sdk-5.2.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      723 2023-05-22 16:30:13.993000 semantha_sdk-5.2.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      507 2023-05-22 16:30:14.014000 semantha_sdk-5.2.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      628 2023-05-22 16:30:14.042000 semantha_sdk-5.2.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1004 2023-05-22 16:30:14.040000 semantha_sdk-5.2.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      503 2023-05-22 16:30:14.007000 semantha_sdk-5.2.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      498 2023-05-22 16:30:13.992000 semantha_sdk-5.2.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      564 2023-05-22 16:30:13.971000 semantha_sdk-5.2.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      447 2023-05-22 16:30:13.999000 semantha_sdk-5.2.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      597 2023-05-22 16:30:14.032000 semantha_sdk-5.2.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      729 2023-05-22 16:30:14.028000 semantha_sdk-5.2.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      536 2023-05-22 16:30:14.006000 semantha_sdk-5.2.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      842 2023-05-22 16:30:14.038000 semantha_sdk-5.2.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      512 2023-05-22 16:30:14.015000 semantha_sdk-5.2.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      498 2023-05-22 16:30:13.958000 semantha_sdk-5.2.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      524 2023-05-22 16:30:14.012000 semantha_sdk-5.2.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      839 2023-05-22 16:30:13.962000 semantha_sdk-5.2.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      531 2023-05-22 16:30:14.013000 semantha_sdk-5.2.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      408 2023-05-22 16:30:13.978000 semantha_sdk-5.2.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      474 2023-05-22 16:30:14.031000 semantha_sdk-5.2.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      576 2023-05-22 16:30:14.035000 semantha_sdk-5.2.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      483 2023-05-22 16:30:13.997000 semantha_sdk-5.2.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      582 2023-05-22 16:30:14.009000 semantha_sdk-5.2.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      499 2023-05-22 16:30:13.989000 semantha_sdk-5.2.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      493 2023-05-22 16:30:14.048000 semantha_sdk-5.2.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      430 2023-05-22 16:30:13.990000 semantha_sdk-5.2.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      528 2023-05-22 16:30:13.998000 semantha_sdk-5.2.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1482 2023-05-22 16:30:14.018000 semantha_sdk-5.2.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      485 2023-05-22 16:30:13.981000 semantha_sdk-5.2.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      787 2023-05-22 16:30:14.003000 semantha_sdk-5.2.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      528 2023-05-22 16:30:14.024000 semantha_sdk-5.2.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0      948 2023-05-22 16:30:13.969000 semantha_sdk-5.2.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      486 2023-05-22 16:30:13.965000 semantha_sdk-5.2.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      493 2023-05-22 16:30:14.010000 semantha_sdk-5.2.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      577 2023-05-22 16:30:13.973000 semantha_sdk-5.2.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      445 2023-05-22 16:30:14.036000 semantha_sdk-5.2.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      775 2023-05-22 16:30:14.030000 semantha_sdk-5.2.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      728 2023-05-22 16:30:14.046000 semantha_sdk-5.2.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      646 2023-05-22 16:30:13.995000 semantha_sdk-5.2.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.2.0/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      873 2023-05-22 16:30:14.023000 semantha_sdk-5.2.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      518 2023-05-22 16:30:13.996000 semantha_sdk-5.2.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      792 2023-05-22 16:30:13.976000 semantha_sdk-5.2.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1669 2023-05-22 16:30:14.022000 semantha_sdk-5.2.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      454 2023-05-22 16:30:13.979000 semantha_sdk-5.2.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      695 2023-05-22 16:30:13.974000 semantha_sdk-5.2.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      851 2023-05-22 16:30:14.011000 semantha_sdk-5.2.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      608 2023-05-22 16:30:13.970000 semantha_sdk-5.2.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      480 2023-05-22 16:30:13.991000 semantha_sdk-5.2.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      542 2023-05-22 16:30:13.963000 semantha_sdk-5.2.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      466 2023-05-22 16:30:13.997000 semantha_sdk-5.2.0/semantha_sdk/model/table.py
--rw-r--r--   0        0        0      565 2023-05-22 16:30:13.982000 semantha_sdk-5.2.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      462 2023-05-22 16:30:14.033000 semantha_sdk-5.2.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      464 2023-05-22 16:30:13.983000 semantha_sdk-5.2.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.2.0/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.2.0/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.2.0/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.2.0/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.2.0/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.2.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.2.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0     8563 1970-01-01 00:00:00.000000 semantha_sdk-5.2.0/setup.py
--rw-r--r--   0        0        0     8322 1970-01-01 00:00:00.000000 semantha_sdk-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.3.0/LICENSE
+-rw-r--r--   0        0        0     1618 2023-06-01 10:22:16.570565 semantha_sdk-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7795 2023-06-01 10:21:34.644458 semantha_sdk-5.3.0/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.3.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.3.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1634 2023-06-01 08:29:07.930000 semantha_sdk-5.3.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0      930 2023-06-01 08:29:07.488000 semantha_sdk-5.3.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      729 2023-06-01 08:29:07.509000 semantha_sdk-5.3.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      739 2023-06-01 08:29:07.718000 semantha_sdk-5.3.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1628 2023-06-01 08:29:07.588000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1493 2023-06-01 08:29:07.539000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3671 2023-06-01 08:29:07.677000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3423 2023-06-01 08:29:07.710000 semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1191 2023-06-01 08:29:07.755000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      832 2023-06-01 08:29:07.775000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1730 2023-06-01 08:29:07.765000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1577 2023-06-01 08:29:07.793000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2722 2023-06-01 08:29:07.744000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      726 2023-06-01 08:29:07.726000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1509 2023-06-01 08:29:07.801000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1508 2023-06-01 08:29:07.820000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1216 2023-06-01 08:29:07.830000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1111 2023-06-01 08:29:07.837000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1170 2023-06-01 08:29:07.846000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0      976 2023-06-01 08:29:07.785000 semantha_sdk-5.3.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     5667 2023-06-01 08:29:08.061000 semantha_sdk-5.3.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1050 2023-06-01 08:29:07.857000 semantha_sdk-5.3.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1369 2023-06-01 08:29:07.881000 semantha_sdk-5.3.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     2315 2023-06-01 08:29:07.950000 semantha_sdk-5.3.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1387 2023-06-01 08:29:07.972000 semantha_sdk-5.3.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1823 2023-06-01 08:29:07.960000 semantha_sdk-5.3.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3566 2023-06-01 08:29:07.990000 semantha_sdk-5.3.0/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     3497 2023-06-01 08:29:08.005000 semantha_sdk-5.3.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     4161 2023-06-01 08:29:07.915000 semantha_sdk-5.3.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1013 2023-06-01 08:29:07.890000 semantha_sdk-5.3.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      791 2023-06-01 08:29:08.258000 semantha_sdk-5.3.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1648 2023-06-01 08:29:08.270000 semantha_sdk-5.3.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1529 2023-06-01 08:29:08.280000 semantha_sdk-5.3.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1545 2023-06-01 08:29:08.333000 semantha_sdk-5.3.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0      762 2023-06-01 08:29:08.287000 semantha_sdk-5.3.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     1524 2023-06-01 08:29:08.309000 semantha_sdk-5.3.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      706 2023-06-01 08:29:08.299000 semantha_sdk-5.3.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0      777 2023-06-01 08:29:08.359000 semantha_sdk-5.3.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      774 2023-06-01 08:29:08.365000 semantha_sdk-5.3.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1514 2023-06-01 08:29:08.351000 semantha_sdk-5.3.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1107 2023-06-01 08:29:08.014000 semantha_sdk-5.3.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     2315 2023-06-01 08:29:08.024000 semantha_sdk-5.3.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1546 2023-06-01 08:29:08.068000 semantha_sdk-5.3.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1494 2023-06-01 08:29:08.108000 semantha_sdk-5.3.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      682 2023-06-01 08:29:08.100000 semantha_sdk-5.3.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0    14477 2023-05-11 17:26:57.378270 semantha_sdk-5.3.0/semantha_sdk/api/reference_documents.py
+-rw-r--r--   0        0        0     2074 2023-06-01 08:29:08.094000 semantha_sdk-5.3.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0     8930 2023-06-01 08:29:08.047000 semantha_sdk-5.3.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0     6565 2023-06-01 08:29:08.149000 semantha_sdk-5.3.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      789 2023-06-01 08:29:07.866000 semantha_sdk-5.3.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.3.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.3.0/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      836 2023-06-01 08:29:08.122000 semantha_sdk-5.3.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      676 2023-06-01 08:29:08.114000 semantha_sdk-5.3.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1379 2023-06-01 08:29:08.158000 semantha_sdk-5.3.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5389 2023-06-01 08:29:08.174000 semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4015 2023-06-01 08:29:08.199000 semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      844 2023-06-01 08:29:08.077000 semantha_sdk-5.3.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0      840 2023-06-01 08:29:08.220000 semantha_sdk-5.3.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1115 2023-06-01 08:29:08.230000 semantha_sdk-5.3.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0      912 2023-06-01 08:29:08.210000 semantha_sdk-5.3.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1310 2023-06-01 08:29:08.248000 semantha_sdk-5.3.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     4241 2023-06-01 08:29:09.369000 semantha_sdk-5.3.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-01 08:29:08.744000 semantha_sdk-5.3.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      654 2023-06-01 08:29:08.982000 semantha_sdk-5.3.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      556 2023-06-01 08:29:08.895000 semantha_sdk-5.3.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      535 2023-06-01 08:29:09.185000 semantha_sdk-5.3.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      546 2023-06-01 08:29:08.875000 semantha_sdk-5.3.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      930 2023-06-01 08:29:08.889000 semantha_sdk-5.3.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      508 2023-06-01 08:29:08.779000 semantha_sdk-5.3.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      672 2023-06-01 08:29:08.964000 semantha_sdk-5.3.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0     1139 2023-06-01 08:29:08.852000 semantha_sdk-5.3.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      516 2023-06-01 08:29:09.034000 semantha_sdk-5.3.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      604 2023-06-01 08:29:09.256000 semantha_sdk-5.3.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      476 2023-06-01 08:29:09.024000 semantha_sdk-5.3.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      519 2023-06-01 08:29:09.003000 semantha_sdk-5.3.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1213 2023-06-01 08:29:09.247000 semantha_sdk-5.3.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0      939 2023-06-01 08:29:09.159000 semantha_sdk-5.3.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      723 2023-06-01 08:29:09.098000 semantha_sdk-5.3.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      566 2023-06-01 08:29:08.773000 semantha_sdk-5.3.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      628 2023-06-01 08:29:08.971000 semantha_sdk-5.3.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1004 2023-06-01 08:29:09.123000 semantha_sdk-5.3.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      503 2023-06-01 08:29:09.011000 semantha_sdk-5.3.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      498 2023-06-01 08:29:08.737000 semantha_sdk-5.3.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      564 2023-06-01 08:29:08.701000 semantha_sdk-5.3.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      447 2023-06-01 08:29:09.107000 semantha_sdk-5.3.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      597 2023-06-01 08:29:08.795000 semantha_sdk-5.3.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      729 2023-06-01 08:29:08.991000 semantha_sdk-5.3.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      536 2023-06-01 08:29:09.029000 semantha_sdk-5.3.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      842 2023-06-01 08:29:08.946000 semantha_sdk-5.3.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      512 2023-06-01 08:29:08.997000 semantha_sdk-5.3.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      498 2023-06-01 08:29:08.921000 semantha_sdk-5.3.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      524 2023-06-01 08:29:08.956000 semantha_sdk-5.3.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      839 2023-06-01 08:29:09.071000 semantha_sdk-5.3.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      531 2023-06-01 08:29:08.732000 semantha_sdk-5.3.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      408 2023-06-01 08:29:08.878000 semantha_sdk-5.3.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      474 2023-06-01 08:29:08.924000 semantha_sdk-5.3.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      576 2023-06-01 08:29:08.840000 semantha_sdk-5.3.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      483 2023-06-01 08:29:08.784000 semantha_sdk-5.3.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      582 2023-06-01 08:29:08.692000 semantha_sdk-5.3.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      499 2023-06-01 08:29:08.809000 semantha_sdk-5.3.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      493 2023-06-01 08:29:08.708000 semantha_sdk-5.3.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      430 2023-06-01 08:29:08.632000 semantha_sdk-5.3.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      528 2023-06-01 08:29:08.915000 semantha_sdk-5.3.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1482 2023-06-01 08:29:08.761000 semantha_sdk-5.3.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      485 2023-06-01 08:29:08.901000 semantha_sdk-5.3.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      787 2023-06-01 08:29:08.908000 semantha_sdk-5.3.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      528 2023-06-01 08:29:08.868000 semantha_sdk-5.3.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0      948 2023-06-01 08:29:09.134000 semantha_sdk-5.3.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      486 2023-06-01 08:29:09.102000 semantha_sdk-5.3.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      493 2023-06-01 08:29:09.138000 semantha_sdk-5.3.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      577 2023-06-01 08:29:08.802000 semantha_sdk-5.3.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      445 2023-06-01 08:29:09.018000 semantha_sdk-5.3.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      775 2023-06-01 08:29:09.050000 semantha_sdk-5.3.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      728 2023-06-01 08:29:08.626000 semantha_sdk-5.3.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      646 2023-06-01 08:29:09.218000 semantha_sdk-5.3.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.3.0/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      873 2023-06-01 08:29:09.086000 semantha_sdk-5.3.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      518 2023-06-01 08:29:08.814000 semantha_sdk-5.3.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      792 2023-06-01 08:29:08.864000 semantha_sdk-5.3.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1669 2023-06-01 08:29:08.834000 semantha_sdk-5.3.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      454 2023-06-01 08:29:08.932000 semantha_sdk-5.3.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      695 2023-06-01 08:29:09.038000 semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      851 2023-06-01 08:29:08.724000 semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      608 2023-06-01 08:29:08.669000 semantha_sdk-5.3.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      480 2023-06-01 08:29:08.788000 semantha_sdk-5.3.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      542 2023-06-01 08:29:08.647000 semantha_sdk-5.3.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      466 2023-06-01 08:29:08.715000 semantha_sdk-5.3.0/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      565 2023-06-01 08:29:09.165000 semantha_sdk-5.3.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      462 2023-06-01 08:29:08.750000 semantha_sdk-5.3.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      464 2023-06-01 08:29:08.680000 semantha_sdk-5.3.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.3.0/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.3.0/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.3.0/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.3.0/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.3.0/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.3.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.3.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0     8464 1970-01-01 00:00:00.000000 semantha_sdk-5.3.0/PKG-INFO
```

### Comparing `semantha_sdk-5.2.0/LICENSE` & `semantha_sdk-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/pyproject.toml` & `semantha_sdk-5.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.2.0"
+version = "5.3.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
@@ -20,38 +20,37 @@
 optional = true
 
 [tool.poetry.group.build]
 optional = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "2.30.0"
+requests = "2.31.0"
 marshmallow = "3.19.0"
 marshmallow-dataclass = "8.5.14"
 pyhumps = "3.8.0"
 
 [tool.poetry.group.unittest.dependencies]
-coverage = "7.2.5"
+coverage = "7.2.7"
 pytest = "7.3.1"
-pytest-cov = "4.0.0"
+pytest-cov = "4.1.0"
 toml = "0.10.2"
 parameterized = "^0.9.0"
 
 [tool.poetry.group.build.dependencies]
-pip-licenses = "4.3.1"
+pip-licenses = "4.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "tt-nexus-pypi-proxy"
 url = "https://tt-yojrlnvtnc.thingsthinking.systems/repository/pypi-org-proxy/simple/"
-default = true
-secondary = false
+priority = "default"
 
 
 [project.dependencies]
 
 [project]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `semantha_sdk-5.2.0/README.md` & `semantha_sdk-5.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
+### Version 5.3.0
+
+Added new service: /api/domains/{domainid}/answers with retrieval augemented answer generation based on your library entries.
+Added new parameter on /modelinstances
+
 ### Version 5.2.0
 
 The SDK is now automatically generated from our openapi.json specification. It covers 71/169 (=42%) of all available services. Many class names and package names have been changed.
 
 ### Version 4.5.0
 Major restructuring of the SDK.
 All sub-resources are directly accessible (instead of invoking getters).
@@ -39,31 +44,37 @@
 
 ## Example Usage
 
 ### Authentication with key
 
 ```
 import semantha_sdk
-api = semantha_sdk.login(server_url="<semantha platform server URL>", key="<your key>")
+api = semantha_sdk.login(server_url="<semantha server URL>", key="<your key>")
 print("Talking to semantha server: " + api.info.get().version)
 ```
 
 ### Authentication with key file
 
 ```
 import semantha_sdk
-api = semantha_sdk.login(server_url="<semantha platform server URL>", key_file="<path to your key file (json format)>")
+api = semantha_sdk.login(server_url="<semantha server URL>", key_file="<path to your key file (json format)>")
 # end-points (resp. resources) can be used like objects
 my_domain = api.domains("my_domain")
 # they may have sub-resources, which can be retrieved as objects as well
 reference_documents = my_domain.referencedocuments
 # GET all reference documents
 print("Library contains "+ len(reference_documents.get()) + " entries")
 ```
 
+Example key file in json format:
+
+```
+{ "API_Key" : "<your key>" }
+```
+
 ### CRUD on End-points
 
 ```
 # CRUD operations are functions
 domain_settings = my_domain.settings.get()
 #Warning: this deletes ALL reference documents/library entries
 my_domain.referencedocuments.delete() 
@@ -164,25 +175,23 @@
               - [x] delete
         - [x] .validation -> SemanticModel
     - [ ] .model
       - [x] .domains("domain_name")
         - [x] .boostwords -> Boostwords
             - [x] get -> list[Boostword]
             - [X] delete -> None
-            - [X] post_word -> Boostword
-            - [X] post_regex -> Boostword
+            - [X] post -> Boostword
         - [x] .boostwords("id") -> Boostword
             - [X] get -> Boostword
             - [X] delete -> None
-            - [X] put_word -> Boostword
-            - [X] put_regex -> Boostword
+            - [X] put -> Boostword
         - [x] .synonyms -> Synonyms
             - [X] get -> list[Synonym]
             - [X] delete -> None
-            - [X] post_word -> Synonym
-            - [X] post_regex -> Synonym
+            - [X] post -> Synonym
         - [x] .synonyms("id") -> Synonym
             - [X] get -> Synonym
             - [X] delete -> None
-            - [X] put_word -> Synonym
-            - [X] put_regex -> Synonym
-        - [x] .datatypes -> list[str]
+            - [X] put -> Synonym
+        - [x] .datatypes -> list[str]
+        - [x] .extractortypes -> list[str]
+        - [x] .metadatatypes -> list[str]
```

### Comparing `semantha_sdk-5.2.0/semantha_sdk/__init__.py` & `semantha_sdk-5.3.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulk.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.3.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/clusters.py` & `semantha_sdk-5.3.0/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.3.0/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/diff.py` & `semantha_sdk-5.3.0/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.3.0/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.3.0/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.3.0/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.3.0/semantha_sdk/api/documentcomparisons.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/documents.py` & `semantha_sdk-5.3.0/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/domain.py` & `semantha_sdk-5.3.0/semantha_sdk/api/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from semantha_sdk.api.answers import AnswersEndpoint
 from semantha_sdk.api.documentannotations import DocumentannotationsEndpoint
 from semantha_sdk.api.documentclasses import DocumentclassesEndpoint
 from semantha_sdk.api.documentcomparisons import DocumentcomparisonsEndpoint
 from semantha_sdk.api.documents import DocumentsEndpoint
 from semantha_sdk.api.modelclasses import ModelclassesEndpoint
 from semantha_sdk.api.modelinstances import ModelinstancesEndpoint
 from semantha_sdk.api.referencedocuments import ReferencedocumentsEndpoint
@@ -32,14 +33,15 @@
         q_params = {}
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DomainSchema)
 
 
     def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
         super().__init__(session, parent_endpoint)
         self._domainname=domainname
+        self.__answers = AnswersEndpoint(session, self._endpoint)
         self.__documentannotations = DocumentannotationsEndpoint(session, self._endpoint)
         self.__documentclasses = DocumentclassesEndpoint(session, self._endpoint)
         self.__documentcomparisons = DocumentcomparisonsEndpoint(session, self._endpoint)
         self.__documents = DocumentsEndpoint(session, self._endpoint)
         self.__modelclasses = ModelclassesEndpoint(session, self._endpoint)
         self.__modelinstances = ModelinstancesEndpoint(session, self._endpoint)
         self.__referencedocuments = ReferencedocumentsEndpoint(session, self._endpoint)
@@ -47,14 +49,19 @@
         self.__settings = SettingsEndpoint(session, self._endpoint)
         self.__similaritymatrix = SimilaritymatrixEndpoint(session, self._endpoint)
         self.__tags = TagsEndpoint(session, self._endpoint)
         self.__validation = ValidationEndpoint(session, self._endpoint)
 
 
     @property
+    def answers(self) -> AnswersEndpoint:
+        return self.__answers
+
+
+    @property
     def documentannotations(self) -> DocumentannotationsEndpoint:
         return self.__documentannotations
 
 
     @property
     def documentclasses(self) -> DocumentclassesEndpoint:
         return self.__documentclasses
```

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/domains.py` & `semantha_sdk-5.3.0/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/info.py` & `semantha_sdk-5.3.0/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/languages.py` & `semantha_sdk-5.3.0/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.3.0/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.3.0/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.3.0/semantha_sdk/api/modelinstances.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,27 @@
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/modelinstances"
 
     def post(self
         , file: IOBase = None
         , documentextractor: str = None
+        , applymatchersfordocumentextractor: bool = None
         , withimages: bool = None
         , withdocument: bool = None
         , withadditionalroots: bool = None
         , documenttype: str = None
         , uilanguage: str = None
         ) -> SemanticModel:
         """
         Extract semantic model for a list of documents
         Args:
             file (IOBase): Input document (left document).
             documentextractor (str): The document extractor you want to be considered.
+            applymatchersfordocumentextractor (bool): 
             
         """
         q_params = {}
         if withimages is not None:
             q_params["withimages"] = withimages
         if withdocument is not None:
             q_params["withdocument"] = withdocument
@@ -41,15 +43,16 @@
             q_params["uilanguage"] = uilanguage
         response = self._session.post(
             url=self._endpoint,
             
             body={
             
                 "file": file,
-                "documentextractor": documentextractor
+                "documentextractor": documentextractor,
+                "applymatchersfordocumentextractor": applymatchersfordocumentextractor
             },
             
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(SemanticModelSchema)
```

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.3.0/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.3.0/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.3.0/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/reference_documents.py` & `semantha_sdk-5.3.0/semantha_sdk/api/reference_documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.3.0/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.3.0/semantha_sdk/api/referencedocuments.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,71 +15,71 @@
     """ author semantha, this is a generated class do not change manually! """
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/referencedocuments"
 
     def get(self
+        , tags: str = None
         , documentids: str = None
         , name: str = None
         , createdafter: int = None
         , createdbefore: int = None
         , updatedafter: int = None
         , updatedbefore: int = None
-        , tags: str = None
         , documentclassids: str = None
         , withoutdocumentclass: bool = None
         , mincharacters: int = None
         , metadata: str = None
         , comment: str = None
         , offset: int = None
         , limit: int = None
         , sort: str = None
         , fields: str = None
         ) -> ReferenceDocumentsResponseContainer:
         """
         Get all reference documents
         Please be aware that this service is limited: The query parameter ‚tags‘ can only be used in combination with an JSON export. 
         Args:
+            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
             documentids (str): List of document Ids for target. The limit here is 65000 IDs.
         The IDs are passed as a JSON array.
             name (str): The document name in your library (in contrast to the file name being used during upload).
             createdafter (int): Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
             createdbefore (int): Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
             updatedafter (int): 
             updatedbefore (int): 
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
             documentclassids (str): List of documentclass IDs for the target. The limit here is 1000 IDs.
         The IDs are passed as a JSON array.
         This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
             withoutdocumentclass (bool): Use this parameter to filter the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
             mincharacters (int): 
             metadata (str): Filter by metadata
             comment (str): Use this parameter to add a comment to your reference document.
             offset (int): Specify from which number on reference documents should be returned.
             limit (int): Specify the number of reference documents to be returned.
             sort (str): Sort the returned reference documents by name, created, updated and/or metadata. Add a - before the field name to sort in descending order.
             fields (str): Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: id, name, tags, metadata, filename, created, processed, lang, updated.
             
         """
         q_params = {}
+        if tags is not None:
+            q_params["tags"] = tags
         if documentids is not None:
             q_params["documentids"] = documentids
         if name is not None:
             q_params["name"] = name
         if createdafter is not None:
             q_params["createdafter"] = createdafter
         if createdbefore is not None:
             q_params["createdbefore"] = createdbefore
         if updatedafter is not None:
             q_params["updatedafter"] = updatedafter
         if updatedbefore is not None:
             q_params["updatedbefore"] = updatedbefore
-        if tags is not None:
-            q_params["tags"] = tags
         if documentclassids is not None:
             q_params["documentclassids"] = documentclassids
         if withoutdocumentclass is not None:
             q_params["withoutdocumentclass"] = withoutdocumentclass
         if mincharacters is not None:
             q_params["mincharacters"] = mincharacters
         if metadata is not None:
```

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/references.py` & `semantha_sdk-5.3.0/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/roles.py` & `semantha_sdk-5.3.0/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.3.0/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/sentence.py` & `semantha_sdk-5.3.0/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/sentences.py` & `semantha_sdk-5.3.0/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/settings.py` & `semantha_sdk-5.3.0/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.3.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/statistic.py` & `semantha_sdk-5.3.0/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/tag.py` & `semantha_sdk-5.3.0/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.3.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/tags.py` & `semantha_sdk-5.3.0/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/api/validation.py` & `semantha_sdk-5.3.0/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/__init__.py` & `semantha_sdk-5.3.0/semantha_sdk/model/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """ author semantha, this is a generated file do not change manually! """
 
 from .annotation_cell import AnnotationCell, AnnotationCellSchema
 from .annotation_page import AnnotationPage, AnnotationPageSchema
+from .answer import Answer, AnswerSchema
+from .answer_reference import AnswerReference, AnswerReferenceSchema
 from .boost_word import BoostWord, BoostWordSchema
 from .class_bulk import ClassBulk, ClassBulkSchema
 from .clustered_document import ClusteredDocument, ClusteredDocumentSchema
 from .clustering_response import ClusteringResponse, ClusteringResponseSchema
 from .complex_property import ComplexProperty, ComplexPropertySchema
 from .current_user import CurrentUser, CurrentUserSchema
 from .data_property import DataProperty, DataPropertySchema
```

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.3.0/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.3.0/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.3.0/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.3.0/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.3.0/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.3.0/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/current_user.py` & `semantha_sdk-5.3.0/semantha_sdk/model/current_user.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/data_property.py` & `semantha_sdk-5.3.0/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/distance.py` & `semantha_sdk-5.3.0/semantha_sdk/model/distance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/document.py` & `semantha_sdk-5.3.0/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/document_class.py` & `semantha_sdk-5.3.0/semantha_sdk/model/document_class.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 @dataclass(frozen=True)
 class DocumentClass(SemanthaModelEntity):
 	""" author semantha, this is a generated class do not change manually! """
 	id: Optional[str]
 	name: str
 	parent_id: Optional[str]
+	metadata: Optional[str]
+	documents_count: Optional[int]
 	sub_classes: Optional[List[DocumentClassNode]]
 	tags: Optional[List[str]]
 	derived_tags: Optional[List[str]]
 	color: Optional[str]
 	derived_color: Optional[str]
 	comment: Optional[str]
 	derived_comment: Optional[str]
 	created: Optional[int]
 	updated: Optional[int]
-	metadata: Optional[str]
 	derived_metadata: Optional[str]
-	documents_count: Optional[int]
 	
 	
 DocumentClassSchema = class_schema(DocumentClass, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.3.0/semantha_sdk/model/document_class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.3.0/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/document_information.py` & `semantha_sdk-5.3.0/semantha_sdk/model/document_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/domain.py` & `semantha_sdk-5.3.0/semantha_sdk/model/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.3.0/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.3.0/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.3.0/semantha_sdk/model/extraction_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/features.py` & `semantha_sdk-5.3.0/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.3.0/semantha_sdk/model/file_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/info.py` & `semantha_sdk-5.3.0/semantha_sdk/model/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/instance.py` & `semantha_sdk-5.3.0/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.3.0/semantha_sdk/model/instance_child.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.3.0/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.3.0/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/model_class.py` & `semantha_sdk-5.3.0/semantha_sdk/model/model_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.3.0/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/page.py` & `semantha_sdk-5.3.0/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/page_content.py` & `semantha_sdk-5.3.0/semantha_sdk/model/page_content.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.3.0/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/process_information.py` & `semantha_sdk-5.3.0/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/reference.py` & `semantha_sdk-5.3.0/semantha_sdk/model/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.3.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-5.3.0/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.3.0/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.3.0/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.3.0/semantha_sdk/model/semi_super_vised_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/sentence.py` & `semantha_sdk-5.3.0/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/settings.py` & `semantha_sdk-5.3.0/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.3.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/statistic.py` & `semantha_sdk-5.3.0/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/synonym.py` & `semantha_sdk-5.3.0/semantha_sdk/model/synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.3.0/semantha_sdk/model/table_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.3.0/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.3.0/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.3.0/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.2.0/setup.py` & `semantha_sdk-5.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,220 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['semantha_sdk',
- 'semantha_sdk.api',
- 'semantha_sdk.model',
- 'semantha_sdk.request',
- 'semantha_sdk.response',
- 'semantha_sdk.rest']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['marshmallow-dataclass==8.5.14',
- 'marshmallow==3.19.0',
- 'pyhumps==3.8.0',
- 'requests==2.30.0']
-
-setup_kwargs = {
-    'name': 'semantha-sdk',
-    'version': '5.2.0',
-    'description': 'This is a python client sdk for accessing semantha (the semantic platform)',
-    'long_description': '![](https://www.semantha.de/wp-content/uploads/semantha-inverted.svg)\n\n# semantha® SDK\n\nThe semantha SDK is a high-level REST client to access the [semantha](http://semantha.ai) API.\nThe SDK is still under development.\nAn overview of the current progress (i.e. implemented and tested resources and endpoints) may be found at the end of\nthis document (State of Development).\nThe semantha SDK is compatible with python >= 3.8.\n\n## Design guideline/idea\nEvery api call can easily be translated into a python sdk call:\n`GET /api/info -> api.info.get()`\nThe SDK offers type hints and doc strings for services, parameters, input types and return types within your IDE.\n\n### Disclaimer\n\n**IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.\nUse with caution and on own risk.\n\n## Update Notes\n\n### Version 5.2.0\n\nThe SDK is now automatically generated from our openapi.json specification. It covers 71/169 (=42%) of all available services. Many class names and package names have been changed.\n\n### Version 4.5.0\nMajor restructuring of the SDK.\nAll sub-resources are directly accessible (instead of invoking getters).\nThat also means that (except for a few) all functions are plain get/post/delete/put/patch.\nFor example, in Versions < 4.5.0 a domain resource was fetched using `semantha_sdk.domains.get_one("domain_name")`.\nStarting with 4.5.0 it is `semantha_sdk.domains("domain_name")`.\nThat also means that get/post/put/patch functions return semantha model objects (and never resources), which makes usage more consistent.\n\n### Access\n\nTo access semantha\'s API you will need an API and a server url.\nBoth can be requested via [this contact form](https://www.semantha.de/request/).\n\n## Example Usage\n\n### Authentication with key\n\n```\nimport semantha_sdk\napi = semantha_sdk.login(server_url="<semantha platform server URL>", key="<your key>")\nprint("Talking to semantha server: " + api.info.get().version)\n```\n\n### Authentication with key file\n\n```\nimport semantha_sdk\napi = semantha_sdk.login(server_url="<semantha platform server URL>", key_file="<path to your key file (json format)>")\n# end-points (resp. resources) can be used like objects\nmy_domain = api.domains("my_domain")\n# they may have sub-resources, which can be retrieved as objects as well\nreference_documents = my_domain.referencedocuments\n# GET all reference documents\nprint("Library contains "+ len(reference_documents.get()) + " entries")\n```\n\n### CRUD on End-points\n\n```\n# CRUD operations are functions\ndomain_settings = my_domain.settings.get()\n#Warning: this deletes ALL reference documents/library entries\nmy_domain.referencedocuments.delete() \n```\n\n### Function Return Types & semantha Data Model\n\n```\n# some functions only return None, e.g.\nmy_domain.referencedocuments.delete() # returns NoneType\n\n# others return built in types, e.g\nroles_list = currentuser.roles.get() # returns List[str]\n\n# but most return objects of the semantha Data Model\n# (all returned objects are instances of frozen dataclasses)\nsettings = my_domain.settings.get() # returns instance of Settings\n# attributes can be accessed as properties, e.g.\nsettings.enable_tagging # returns true or false\n# Data Model objects may be complex\ndocument = my_domain.references.post(file=a, referencedocument=b) # returns instance of Document\n# the following returns the similarity value of the first references of the first sentence of the\n# the first paragraph on the first page of the document (if a reference was found for this sentence)\nsimilarity = pages[0].contents[0].paragraphs[0].references[0].similarity # returns float\n```\n\n## State of Development\n\nThe following resources and end-points are fully functional and (partially) tested:\n\n- [X] login -> API\n    - [X] .currentuser -> CurrentUser\n        - [X] get -> CurrentUser\n        - [X] roles -> RolesEndpoint\n          - [x] get -> List[str]\n    - [X] .diff -> Diff\n        - [X] post -> List[Difference]\n    - [X] .info -> InfoEndpoint\n        - [X] get -> Info\n    - [x] .languages -> List[str]\n    - [X] .domains -> Domains\n        - [X] get -> List[Domain]\n    - [X] .domains("domain_name") -> Domain\n        - [X] .documentannotations -> DocumentAnnotationsEndpoint\n            - [X] post -> IOBase\n        - [X] .documentclasses -> DocumentclassesEndpoint\n            - [X] get -> List[DocumentClass]\n            - [X] post -> DocumentClass\n            - [X] delete -> None\n        - [X] .documentclasses("id") -> DocumentclassEndpoint\n            - [X] get -> DocumentClass(\n            - [X] delete -> None\n            - [X] put -> DocumentClass\n            - [ ] documentclasses -> \n                - [ ] get -> List[DocumentClass]\n                - [ ] post -> DocumentClass\n            - [x] referencedocuments -> ReferencedocumentsEndpoint\n                - [x] get -> List[Document]\n                - [x] patch -> None\n                - [x] delete -> None\n        - [X] .documentcomparisons -> DocumentcomparisonsEndpoint\n            - [ ] post ->\n          - [X] .documents -> DocumentsEndpoint\n              - [X] post -> List[Document]\n        - [x] .modelinstances -> ModelInstance\n        - [x] .modelclasses -> ModelClass\n        - [X] .referencedocuments -> ReferenceDocuments\n            - [X] get -> ReferenceDocuments\n            - [X] delete -> None\n            - [X] post -> list[DocumentInformation]\n            - [x] .clusters -> DocumentCluster\n              - [x] get -> DocumentCluster\n            - [x] .statistic -> Statistics\n              - [x] get -> Statistic\n            - [x] .namedentities -> NamedEntities\n              - [x] get -> Optional[NamedEntities]\n        - [x] .referencedocuments("id") -> ReferenceDocument\n            - [X] get -> Document\n            - [X] delete -> None\n            - [X] patch -> DocumentInformation\n            - [X] .paragraphs("id") -> ReferenceDocumentParagraph\n                - [X] get -> Paragraph\n                - [X] patch -> Paragraph\n                - [X] delete -> None\n            - [X] .sentences("id") -> ReferenceDocumentSentence\n                - [x] get -> Sentence\n        - [X] .references -> References\n            - [X] post -> Document\n        - [x] .settings -> DomainSettings\n            - [X] get -> DomainSettings\n            - [X] patch -> DomainSettings\n        - [x] .similaritymatrix -> List[MatrixRow]\n            - [x] .clusters -> List[MatrixRow]\n        - [ ] .tags -> DomainTags\n            - [X] get -> list[str]\n            - .("tag").referencedocuments\n              - [x] get\n              - [x] delete\n        - [x] .validation -> SemanticModel\n    - [ ] .model\n      - [x] .domains("domain_name")\n        - [x] .boostwords -> Boostwords\n            - [x] get -> list[Boostword]\n            - [X] delete -> None\n            - [X] post_word -> Boostword\n            - [X] post_regex -> Boostword\n        - [x] .boostwords("id") -> Boostword\n            - [X] get -> Boostword\n            - [X] delete -> None\n            - [X] put_word -> Boostword\n            - [X] put_regex -> Boostword\n        - [x] .synonyms -> Synonyms\n            - [X] get -> list[Synonym]\n            - [X] delete -> None\n            - [X] post_word -> Synonym\n            - [X] post_regex -> Synonym\n        - [x] .synonyms("id") -> Synonym\n            - [X] get -> Synonym\n            - [X] delete -> None\n            - [X] put_word -> Synonym\n            - [X] put_regex -> Synonym\n        - [x] .datatypes -> list[str]',
-    'author': 'Sebastian Weigelt',
-    'author_email': 'sebastian.weigelt@semantha.ai',
-    'maintainer': 'semantha support',
-    'maintainer_email': 'support@semantha.de',
-    'url': 'https://semantha.de',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: semantha-sdk
+Version: 5.3.0
+Summary: This is a python client sdk for accessing semantha (the semantic platform)
+Home-page: https://semantha.de
+License: Apache-2.0
+Author: Sebastian Weigelt
+Author-email: sebastian.weigelt@semantha.ai
+Maintainer: semantha support
+Maintainer-email: support@semantha.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: marshmallow (==3.19.0)
+Requires-Dist: marshmallow-dataclass (==8.5.14)
+Requires-Dist: pyhumps (==3.8.0)
+Requires-Dist: requests (==2.31.0)
+Description-Content-Type: text/markdown
+
+![](https://www.semantha.de/wp-content/uploads/semantha-inverted.svg)
+
+# semantha® SDK
+
+The semantha SDK is a high-level REST client to access the [semantha](http://semantha.ai) API.
+The SDK is still under development.
+An overview of the current progress (i.e. implemented and tested resources and endpoints) may be found at the end of
+this document (State of Development).
+The semantha SDK is compatible with python >= 3.8.
+
+## Design guideline/idea
+Every api call can easily be translated into a python sdk call:
+`GET /api/info -> api.info.get()`
+The SDK offers type hints and doc strings for services, parameters, input types and return types within your IDE.
+
+### Disclaimer
+
+**IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
+Use with caution and on own risk.
+
+## Update Notes
+
+### Version 5.3.0
+
+Added new service: /api/domains/{domainid}/answers with retrieval augemented answer generation based on your library entries.
+Added new parameter on /modelinstances
+
+### Version 5.2.0
+
+The SDK is now automatically generated from our openapi.json specification. It covers 71/169 (=42%) of all available services. Many class names and package names have been changed.
+
+### Version 4.5.0
+Major restructuring of the SDK.
+All sub-resources are directly accessible (instead of invoking getters).
+That also means that (except for a few) all functions are plain get/post/delete/put/patch.
+For example, in Versions < 4.5.0 a domain resource was fetched using `semantha_sdk.domains.get_one("domain_name")`.
+Starting with 4.5.0 it is `semantha_sdk.domains("domain_name")`.
+That also means that get/post/put/patch functions return semantha model objects (and never resources), which makes usage more consistent.
+
+### Access
+
+To access semantha's API you will need an API and a server url.
+Both can be requested via [this contact form](https://www.semantha.de/request/).
+
+## Example Usage
+
+### Authentication with key
+
+```
+import semantha_sdk
+api = semantha_sdk.login(server_url="<semantha server URL>", key="<your key>")
+print("Talking to semantha server: " + api.info.get().version)
+```
+
+### Authentication with key file
+
+```
+import semantha_sdk
+api = semantha_sdk.login(server_url="<semantha server URL>", key_file="<path to your key file (json format)>")
+# end-points (resp. resources) can be used like objects
+my_domain = api.domains("my_domain")
+# they may have sub-resources, which can be retrieved as objects as well
+reference_documents = my_domain.referencedocuments
+# GET all reference documents
+print("Library contains "+ len(reference_documents.get()) + " entries")
+```
+
+Example key file in json format:
+
+```
+{ "API_Key" : "<your key>" }
+```
+
+### CRUD on End-points
+
+```
+# CRUD operations are functions
+domain_settings = my_domain.settings.get()
+#Warning: this deletes ALL reference documents/library entries
+my_domain.referencedocuments.delete() 
+```
+
+### Function Return Types & semantha Data Model
+
+```
+# some functions only return None, e.g.
+my_domain.referencedocuments.delete() # returns NoneType
+
+# others return built in types, e.g
+roles_list = currentuser.roles.get() # returns List[str]
+
+# but most return objects of the semantha Data Model
+# (all returned objects are instances of frozen dataclasses)
+settings = my_domain.settings.get() # returns instance of Settings
+# attributes can be accessed as properties, e.g.
+settings.enable_tagging # returns true or false
+# Data Model objects may be complex
+document = my_domain.references.post(file=a, referencedocument=b) # returns instance of Document
+# the following returns the similarity value of the first references of the first sentence of the
+# the first paragraph on the first page of the document (if a reference was found for this sentence)
+similarity = pages[0].contents[0].paragraphs[0].references[0].similarity # returns float
+```
+
+## State of Development
+
+The following resources and end-points are fully functional and (partially) tested:
+
+- [X] login -> API
+    - [X] .currentuser -> CurrentUser
+        - [X] get -> CurrentUser
+        - [X] roles -> RolesEndpoint
+          - [x] get -> List[str]
+    - [X] .diff -> Diff
+        - [X] post -> List[Difference]
+    - [X] .info -> InfoEndpoint
+        - [X] get -> Info
+    - [x] .languages -> List[str]
+    - [X] .domains -> Domains
+        - [X] get -> List[Domain]
+    - [X] .domains("domain_name") -> Domain
+        - [X] .documentannotations -> DocumentAnnotationsEndpoint
+            - [X] post -> IOBase
+        - [X] .documentclasses -> DocumentclassesEndpoint
+            - [X] get -> List[DocumentClass]
+            - [X] post -> DocumentClass
+            - [X] delete -> None
+        - [X] .documentclasses("id") -> DocumentclassEndpoint
+            - [X] get -> DocumentClass(
+            - [X] delete -> None
+            - [X] put -> DocumentClass
+            - [ ] documentclasses -> 
+                - [ ] get -> List[DocumentClass]
+                - [ ] post -> DocumentClass
+            - [x] referencedocuments -> ReferencedocumentsEndpoint
+                - [x] get -> List[Document]
+                - [x] patch -> None
+                - [x] delete -> None
+        - [X] .documentcomparisons -> DocumentcomparisonsEndpoint
+            - [ ] post ->
+          - [X] .documents -> DocumentsEndpoint
+              - [X] post -> List[Document]
+        - [x] .modelinstances -> ModelInstance
+        - [x] .modelclasses -> ModelClass
+        - [X] .referencedocuments -> ReferenceDocuments
+            - [X] get -> ReferenceDocuments
+            - [X] delete -> None
+            - [X] post -> list[DocumentInformation]
+            - [x] .clusters -> DocumentCluster
+              - [x] get -> DocumentCluster
+            - [x] .statistic -> Statistics
+              - [x] get -> Statistic
+            - [x] .namedentities -> NamedEntities
+              - [x] get -> Optional[NamedEntities]
+        - [x] .referencedocuments("id") -> ReferenceDocument
+            - [X] get -> Document
+            - [X] delete -> None
+            - [X] patch -> DocumentInformation
+            - [X] .paragraphs("id") -> ReferenceDocumentParagraph
+                - [X] get -> Paragraph
+                - [X] patch -> Paragraph
+                - [X] delete -> None
+            - [X] .sentences("id") -> ReferenceDocumentSentence
+                - [x] get -> Sentence
+        - [X] .references -> References
+            - [X] post -> Document
+        - [x] .settings -> DomainSettings
+            - [X] get -> DomainSettings
+            - [X] patch -> DomainSettings
+        - [x] .similaritymatrix -> List[MatrixRow]
+            - [x] .clusters -> List[MatrixRow]
+        - [ ] .tags -> DomainTags
+            - [X] get -> list[str]
+            - .("tag").referencedocuments
+              - [x] get
+              - [x] delete
+        - [x] .validation -> SemanticModel
+    - [ ] .model
+      - [x] .domains("domain_name")
+        - [x] .boostwords -> Boostwords
+            - [x] get -> list[Boostword]
+            - [X] delete -> None
+            - [X] post -> Boostword
+        - [x] .boostwords("id") -> Boostword
+            - [X] get -> Boostword
+            - [X] delete -> None
+            - [X] put -> Boostword
+        - [x] .synonyms -> Synonyms
+            - [X] get -> list[Synonym]
+            - [X] delete -> None
+            - [X] post -> Synonym
+        - [x] .synonyms("id") -> Synonym
+            - [X] get -> Synonym
+            - [X] delete -> None
+            - [X] put -> Synonym
+        - [x] .datatypes -> list[str]
+        - [x] .extractortypes -> list[str]
+        - [x] .metadatatypes -> list[str]
```

