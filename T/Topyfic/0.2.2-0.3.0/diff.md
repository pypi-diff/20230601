# Comparing `tmp/Topyfic-0.2.2.tar.gz` & `tmp/Topyfic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.2.2.tar", last modified: Thu May 18 22:13:08 2023, max compression
+gzip compressed data, was "Topyfic-0.3.0.tar", last modified: Wed May 31 22:05:06 2023, max compression
```

## Comparing `Topyfic-0.2.2.tar` & `Topyfic-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-18 22:13:08.758843 Topyfic-0.2.2/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.2.2/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-18 22:13:08.758920 Topyfic-0.2.2/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.2.2/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-18 22:13:08.757445 Topyfic-0.2.2/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2022-10-21 21:50:45.000000 Topyfic-0.2.2/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    44549 2023-04-26 18:27:24.000000 Topyfic-0.2.2/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.2.2/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10863 2023-01-20 10:16:01.000000 Topyfic-0.2.2/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    11278 2023-05-01 21:58:44.000000 Topyfic-0.2.2/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10461 2023-03-29 18:16:24.000000 Topyfic-0.2.2/Topyfic/train.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    27627 2023-05-18 22:07:57.000000 Topyfic-0.2.2/Topyfic/utils.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-18 22:13:08.758702 Topyfic-0.2.2/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-18 22:13:08.759188 Topyfic-0.2.2/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1975 2023-05-18 22:09:59.000000 Topyfic-0.2.2/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 22:05:06.173368 Topyfic-0.3.0/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.3.0/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-31 22:05:06.173461 Topyfic-0.3.0/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.3.0/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 22:05:06.171803 Topyfic-0.3.0/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2022-10-21 21:50:45.000000 Topyfic-0.3.0/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    44549 2023-04-26 18:27:24.000000 Topyfic-0.3.0/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.3.0/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    15365 2023-05-31 21:37:09.000000 Topyfic-0.3.0/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    11278 2023-05-01 21:58:44.000000 Topyfic-0.3.0/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10461 2023-03-29 18:16:24.000000 Topyfic-0.3.0/Topyfic/train.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    38341 2023-05-31 21:56:34.000000 Topyfic-0.3.0/Topyfic/utils.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 22:05:06.173223 Topyfic-0.3.0/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-31 22:05:05.000000 Topyfic-0.3.0/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-05-31 22:05:05.000000 Topyfic-0.3.0/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-31 22:05:05.000000 Topyfic-0.3.0/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-31 22:05:05.000000 Topyfic-0.3.0/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-31 22:05:05.000000 Topyfic-0.3.0/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-31 22:05:06.173740 Topyfic-0.3.0/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1997 2023-05-31 22:04:39.000000 Topyfic-0.3.0/setup.py
```

### Comparing `Topyfic-0.2.2/LICENSE.txt` & `Topyfic-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.2/PKG-INFO` & `Topyfic-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.2.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.0.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.2.2/README.md` & `Topyfic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.2/Topyfic/analysis.py` & `Topyfic-0.3.0/Topyfic/analysis.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.2/Topyfic/main.py` & `Topyfic-0.3.0/Topyfic/main.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.2/Topyfic/topModel.py` & `Topyfic-0.3.0/Topyfic/topModel.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import joblib
 import pickle
 import numpy as np
 import pandas as pd
 from sklearn.decomposition import LatentDirichletAllocation
 import matplotlib.pyplot as plt
 import seaborn as sns
+from scipy import stats
 
 sns.set_context('paper')
 warnings.filterwarnings('ignore')
 
 from Topyfic.topic import *
 
 
@@ -241,14 +242,125 @@
         if save:
             plt.savefig(f"{file_name}.{file_format}")
         if show:
             plt.show()
         else:
             plt.close()
 
+    def MA_plot(self,
+                topic1,
+                topic2,
+                pseudocount=1,
+                threshold=1,
+                cutoff=2,
+                consistency_correction=1.4826,
+                labels=None,
+                save=True,
+                show=True,
+                file_format="pdf",
+                file_name="MA_plot"):
+        """
+        plot MA based on the gene weights on given topics
+
+        :param topic1: first topic to be compared
+        :type topic1: str
+        :param topic2: second topic to be compared
+        :type topic2: str
+        :param pseudocount: pseudocount that you want to add (default: 1)
+        :type pseudocount: float
+        :param threshold: threshold to filter genes based on A values (default: 1)
+        :type threshold: float
+        :param cutoff: cutoff for categorized genes by modified z-score (default: 2)
+        :type cutoff: float
+        :param consistency_correction: the factor converts the MAD to the standard deviation for a given distribution. The default value (1.4826) is the conversion factor if the underlying data is normally distributed
+        :type consistency_correction: float
+        :param labels: list of gene names wish to show in MA-plot
+        :type labels: list
+        :param save: indicate if you want to save the plot or not (default: True)
+        :type save: bool
+        :param show: indicate if you want to show the plot or not (default: True)
+        :type show: bool
+        :param file_format: indicate the format of plot (default: pdf)
+        :type file_format: str
+        :param file_name: name and path of the plot use for save (default: MA_plot)
+        :type file_name: str
+
+        :return: return M and A values
+        """
+        gene_weights = self.get_gene_weights()
+        topic1 = gene_weights[topic1]
+        topic2 = gene_weights[topic2]
+
+        topic1 += pseudocount
+        topic2 += pseudocount
+
+        A = (np.log2(topic1) + np.log2(topic2)) / 2
+        M = np.log2(topic1) - np.log2(topic2)
+
+        gene_zscore = pd.concat([A, M], axis=1)
+        gene_zscore.columns = ["A", "M"]
+        gene_zscore = gene_zscore[gene_zscore.A > threshold]
+
+        gene_zscore['mod_zscore'], mad = TopModel.modified_zscore(gene_zscore['M'], consistency_correction=consistency_correction)
+
+        plot_df = gene_zscore.copy(deep=True)
+        plot_df.mod_zscore = plot_df.mod_zscore.abs()
+        plot_df.mod_zscore[plot_df.mod_zscore > cutoff] = cutoff
+        plot_df.mod_zscore[plot_df.mod_zscore < cutoff] = 0
+        plot_df.mod_zscore.fillna(0, inplace=True)
+        plot_df.mod_zscore = plot_df.mod_zscore.astype(int)
+        if labels is not None:
+            plot_df['label'] = plot_df.index.tolist()
+            plot_df.label[~plot_df.label.isin(labels)] = ""
+
+        y = plot_df.M.median()
+        ymin = y - consistency_correction * mad * 2
+        ymax = y + consistency_correction * mad * 2
+        xmin = round(gene_zscore.A.min()) - 1
+        xmax = round(gene_zscore.A.max())
+
+        sns.scatterplot(data=plot_df, x="A", y="M", hue="mod_zscore",
+                        palette=["orchid", "royalblue"])
+
+        if labels is not None:
+            for label in labels:
+                plt.text(plot_df.A[label] - 0.2, plot_df.M[label] + 0.2, label)
+
+        plt.legend(title='abs(Z-score)', loc='upper right', labels=[f'> {cutoff}', f'< {cutoff}'])
+
+        plt.hlines(y=y, xmin=xmin, xmax=xmax, colors="red")
+        plt.hlines(y=ymin, xmin=xmin, xmax=xmax, colors="orange", linestyles='--')
+        plt.hlines(y=ymax, xmin=xmin, xmax=xmax, colors="orange", linestyles='--')
+
+        if save:
+            plt.savefig(f"{file_name}.{file_format}")
+        if show:
+            plt.show()
+        else:
+            plt.close()
+
+        return gene_zscore
+
+    @staticmethod
+    def modified_zscore(data, consistency_correction=1.4826):
+        """
+        Returns the modified z score and Median Absolute Deviation (MAD) from the scores in data.
+        The consistency_correction factor converts the MAD to the standard deviation for a given
+        distribution. The default value (1.4826) is the conversion factor if the underlying data
+        is normally distributed
+        """
+        median = np.median(data)
+
+        deviation_from_med = np.array(data) - median
+
+        mad = np.median(np.abs(deviation_from_med))
+        mod_zscore = deviation_from_med / (consistency_correction * mad)
+
+        return mod_zscore, mad
+
     def save_topModel(self, name=None, save_path=""):
         """
         save TopModel class as a pickle file
 
         :param name: name of the pickle file (default: topModel_TopModel.name)
         :type name: str
         :param save_path: directory you want to use to save pickle file (default is saving near script)
```

### Comparing `Topyfic-0.2.2/Topyfic/topic.py` & `Topyfic-0.3.0/Topyfic/topic.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.2/Topyfic/train.py` & `Topyfic-0.3.0/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.2/Topyfic/utils.py` & `Topyfic-0.3.0/Topyfic/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -684,7 +684,236 @@
         if plot_show:
             plt.show()
         else:
             plt.close()
 
         return axs
 
+    def MA_plot(topic1,
+                topic2,
+                pseudocount=1,
+                threshold=1,
+                cutoff=2,
+                consistency_correction=1.4826,
+                labels=None,
+                save=True,
+                show=True,
+                file_format="pdf",
+                file_name="MA_plot"):
+        """
+        plot MA based on the gene weights on given topics
+
+        :param topic1: first topic to be compared
+        :type topic1: str
+        :param topic2: second topic to be compared
+        :type topic2: str
+        :param pseudocount: pseudocount that you want to add (default: 1)
+        :type pseudocount: float
+        :param threshold: threshold to filter genes based on A values (default: 1)
+        :type threshold: float
+        :param cutoff: cutoff for categorized genes by modified z-score (default: 2)
+        :type cutoff: float
+        :param consistency_correction: the factor converts the MAD to the standard deviation for a given distribution. The default value (1.4826) is the conversion factor if the underlying data is normally distributed
+        :type consistency_correction: float
+        :param labels: list of gene names wish to show in MA-plot
+        :type labels: list
+        :param save: indicate if you want to save the plot or not (default: True)
+        :type save: bool
+        :param show: indicate if you want to show the plot or not (default: True)
+        :type show: bool
+        :param file_format: indicate the format of plot (default: pdf)
+        :type file_format: str
+        :param file_name: name and path of the plot use for save (default: MA_plot)
+        :type file_name: str
+
+        :return: return M and A values
+        """
+        topic1 += pseudocount
+        topic2 += pseudocount
+
+        A = (np.log2(topic1) + np.log2(topic2)) / 2
+        M = np.log2(topic1) - np.log2(topic2)
+
+        gene_zscore = pd.concat([A, M], axis=1)
+        gene_zscore.columns = ["A", "M"]
+        gene_zscore = gene_zscore[gene_zscore.A > threshold]
+
+        gene_zscore['mod_zscore'], mad = modified_zscore(gene_zscore['M'],
+                                                         consistency_correction=consistency_correction)
+
+        plot_df = gene_zscore.copy(deep=True)
+        plot_df.mod_zscore = plot_df.mod_zscore.abs()
+        plot_df.mod_zscore[plot_df.mod_zscore > cutoff] = cutoff
+        plot_df.mod_zscore[plot_df.mod_zscore < cutoff] = 0
+        plot_df.mod_zscore.fillna(0, inplace=True)
+        plot_df.mod_zscore = plot_df.mod_zscore.astype(int)
+        if labels is not None:
+            plot_df['label'] = plot_df.index.tolist()
+            plot_df.label[~plot_df.label.isin(labels)] = ""
+
+        y = plot_df.M.median()
+        ymin = y - consistency_correction * mad * 2
+        ymax = y + consistency_correction * mad * 2
+        xmin = round(gene_zscore.A.min()) - 1
+        xmax = round(gene_zscore.A.max())
+
+        sns.scatterplot(data=plot_df, x="A", y="M", hue="mod_zscore",
+                        palette=["orchid", "royalblue"])
+
+        if labels is not None:
+            for label in labels:
+                plt.text(plot_df.A[label] - 0.2, plot_df.M[label] + 0.2, label)
+
+        plt.legend(title='abs(Z-score)', loc='upper right', labels=[f'> {cutoff}', f'< {cutoff}'])
+
+        plt.hlines(y=y, xmin=xmin, xmax=xmax, colors="red")
+        plt.hlines(y=ymin, xmin=xmin, xmax=xmax, colors="orange", linestyles='--')
+        plt.hlines(y=ymax, xmin=xmin, xmax=xmax, colors="orange", linestyles='--')
+
+        if save:
+            plt.savefig(f"{file_name}.{file_format}")
+        if show:
+            plt.show()
+        else:
+            plt.close()
+
+        return gene_zscore
+
+    def modified_zscore(data, consistency_correction=1.4826):
+        """
+        Returns the modified z score and Median Absolute Deviation (MAD) from the scores in data.
+        The consistency_correction factor converts the MAD to the standard deviation for a given
+        distribution. The default value (1.4826) is the conversion factor if the underlying data
+        is normally distributed
+        """
+        median = np.median(data)
+
+        deviation_from_med = np.array(data) - median
+
+        mad = np.median(np.abs(deviation_from_med))
+        mod_zscore = deviation_from_med / (consistency_correction * mad)
+
+        return mod_zscore, mad
+
+    def functional_enrichment_analysis(gene_list,
+                                       type,
+                                       organism,
+                                       sets=None,
+                                       p_value=0.05,
+                                       file_format="pdf",
+                                       file_name="functional_enrichment_analysis"):
+        """
+        Doing functional enrichment analysis including GO, KEGG and REACTOME
+
+        :param gene_list: list of gene name
+        :type gene_list:list
+        :param type: indicate the type of databases which it should be one of "GO", "REACTOME"
+        :type type: str
+        :param organism: name of the organ you want to do functional enrichment analysis
+        :type organism: str
+        :param sets: str, list, tuple of Enrichr Library name(s). (you can add any Enrichr Libraries from here: https://maayanlab.cloud/Enrichr/#stats) only need to fill if the type is GO
+        :type sets: str, list, tuple
+        :param p_value: Defines the pValue threshold. (default: 0.05)
+        :type p_value: float
+        :param file_format: indicate the format of plot (default: pdf)
+        :type file_format: str
+        :param file_name: name and path of the plot use for save (default: gene_composition)
+        :type file_name: str
+        """
+
+        if type not in ["GO", "REACTOME"]:
+            sys.exit("Type is not valid! it should be one of them GO, KEGG, REACTOME")
+
+        if type == "GO" and sets is None:
+            sets = ["GO_Biological_Process_2021"]
+        elif type == "KEGG" and sets is None:
+            sets = ["KEGG_2016"]
+
+        if type in ["GO", "KEGG"]:
+            enr = gp.enrichr(gene_list=gene_list,
+                             gene_sets=sets,
+                             organism=organism,
+                             outdir=f"{file_name}",
+                             cutoff=p_value)
+            dotplot(enr.res2d,
+                    title=f"Gene ontology",
+                    cmap='viridis_r',
+                    cutoff=p_value,
+                    ofname=f"{file_name}.{file_format}")
+        else:
+            numGeneModule = len(gene_list)
+            genes = ",".join(gene_list)
+            result = analysis.identifiers(ids=genes,
+                                          species=organism,
+                                          p_value=str(p_value))
+            token = result['summary']['token']
+            analysis.report(token,
+                            path=f"{file_name}/",
+                            file=f"{file_name}.{file_format}",
+                            number='50',
+                            species=organism)
+            token_result = analysis.token(token,
+                                          species=organism,
+                                          p_value=str(p_value))
+
+            print(
+                f"{numGeneModule - token_result['identifiersNotFound']} out of {numGeneModule} identifiers in the sample were found in Reactome.")
+            print(
+                f"{token_result['resourceSummary'][0]['pathways']} pathways were hit by at least one of them, which {len(token_result['pathways'])} of them have p-value more than {p_value}.")
+            print(f"Report was saved {file_name}!")
+            print(f"For more information please visit https://reactome.org/PathwayBrowser/#/DTAB=AN&ANALYSIS={token}")
+
+    def GSEA(gene_list,
+             gene_sets='GO_Biological_Process_2021',
+             p_value=0.05,
+             table=True,
+             plot=True,
+             file_format="pdf",
+             file_name="GSEA",
+             **kwargs):
+        """
+        Doing Gene Set Enrichment Analysis on based on the topic weights using GSEAPY package.
+
+        :param gene_list: pandas series with index as a gene names and their ranks/weights as value
+        :type gene_list: pandas series
+        :param gene_sets: Enrichr Library name or .gmt gene sets file or dict of gene sets. (you can add any Enrichr Libraries from here: https://maayanlab.cloud/Enrichr/#stats)
+        :type gene_sets: str, list, tuple
+        :param p_value: Defines the pValue threshold for plotting. (default: 0.05)
+        :type p_value: float
+        :param table: indicate if you want to save all GO terms that passed the threshold as a table (default: True)
+        :type table: bool
+        :param plot: indicate if you want to plot all GO terms that passed the threshold (default: True)
+        :type plot: bool
+        :param file_format: indicate the format of plot (default: pdf)
+        :type file_format: str
+        :param file_name: name and path of the plot use for save (default: gene_composition)
+        :type file_name: str
+        :param kwargs: Argument to pass to gseapy.prerank(). more info: https://gseapy.readthedocs.io/en/latest/run.html?highlight=gp.prerank#gseapy.prerank
+
+        :return: dataframe contains these columns: Term: gene set name, ES: enrichment score, NES: normalized enrichment score, NOM p-val:  Nominal p-value (from the null distribution of the gene set, FDR q-val: FDR qvalue (adjusted False Discory Rate), FWER p-val: Family wise error rate p-values, Tag %: Percent of gene set before running enrichment peak (ES), Gene %: Percent of gene list before running enrichment peak (ES), Lead_genes: leading edge genes (gene hits before running enrichment peak)
+        :rtype: pandas dataframe
+        """
+        gene_list.index = gene_list.index.str.upper()
+
+        pre_res = gp.prerank(rnk=gene_list,
+                             gene_sets=gene_sets,
+                             format=file_format,
+                             no_plot=~plot,
+                             **kwargs)
+
+        pre_res.res2d.sort_values(["NOM p-val"], inplace=True)
+        pre_res.res2d.drop(["Name"], axis=1, inplace=True)
+
+        if table:
+            pre_res.res2d.to_csv(f"{file_name}.csv")
+
+        if plot:
+            res = pre_res.res2d.copy(deep=True)
+            res = res[res['NOM p-val'] < p_value]
+            for term in res.Term:
+                name = term.split("(GO:")[1][:-1]
+                gseaplot(rank_metric=pre_res.ranking,
+                         term=term,
+                         **pre_res.results[term],
+                         ofname=f"{file_name}_GO_{name}.{file_format}")
+
+        return pre_res.res2d
```

### Comparing `Topyfic-0.2.2/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.3.0/Topyfic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.2.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.0.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.2.2/setup.py` & `Topyfic-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.2.2',  # version number
+    version='v0.3.0',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.2.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.0.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
@@ -29,15 +29,16 @@
         'networkx>=2.8.4',
         'numpy>=1.23.2',
         'reactome2py>=3.0.0',
         'scanpy>=1.9.3',
         'scikit_learn>=1.2.2',
         'scipy>=1.9.1',
         'seaborn>=0.11.2',
-        'statsmodels>=0.13.5'
+        'statsmodels>=0.13.5',
+        #'harmonypy'
 
     ],
     classifiers=[  # choose from here: https://pypi.org/classifiers/
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research ',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: MIT License',
```

