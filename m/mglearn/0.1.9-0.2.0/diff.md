# Comparing `tmp/mglearn-0.1.9.tar.gz` & `tmp/mglearn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mglearn-0.1.9.tar", last modified: Mon May 25 21:22:18 2020, max compression
+gzip compressed data, was "mglearn-0.2.0.tar", last modified: Thu Jun  1 02:38:43 2023, max compression
```

## Comparing `mglearn-0.1.9.tar` & `mglearn-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxrwxrwx   0 andy      (1000) andy      (1000)        0 2020-05-25 21:22:18.000000 mglearn-0.1.9/
--rw-rw-rw-   0 andy      (1000) andy      (1000)       51 2020-05-25 21:15:34.000000 mglearn-0.1.9/MANIFEST.in
--rw-rw-rw-   0 andy      (1000) andy      (1000)      365 2020-05-25 21:22:18.000000 mglearn-0.1.9/PKG-INFO
--rw-rw-rw-   0 andy      (1000) andy      (1000)      927 2020-05-25 21:15:34.000000 mglearn-0.1.9/Readme.md
-drwxrwxrwx   0 andy      (1000) andy      (1000)        0 2020-05-25 21:22:18.000000 mglearn-0.1.9/mglearn/
--rw-rw-rw-   0 andy      (1000) andy      (1000)      230 2020-05-25 21:21:31.000000 mglearn-0.1.9/mglearn/__init__.py
-drwxrwxrwx   0 andy      (1000) andy      (1000)        0 2020-05-25 21:22:18.000000 mglearn-0.1.9/mglearn/data/
--rw-rw-rw-   0 andy      (1000) andy      (1000)  3974305 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/data/adult.data
--rw-rw-rw-   0 andy      (1000) andy      (1000)   688092 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/data/citibike.csv
--rw-rw-rw-   0 andy      (1000) andy      (1000)     5822 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/data/ram_price.csv
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1903 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/datasets.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3306 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/make_blobs.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3954 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_2d_separator.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3449 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_agglomerative.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)      890 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_animal_tree.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     8867 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_cross_validation.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1798 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_dbscan.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1067 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_decomposition.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     4157 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_grid_search.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3125 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_helpers.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3172 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_improper_preprocessing.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     2738 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_interactive_tree.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     5791 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_kmeans.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)      944 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_kneighbors_regularization.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1066 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_knn_classification.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1285 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_knn_regression.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1005 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_linear_regression.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1104 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_linear_svc_regularization.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     4121 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_metrics.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3156 2020-05-25 21:17:56.000000 mglearn-0.1.9/mglearn/plot_nmf.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3510 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_nn_graphs.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     4715 2020-05-25 21:20:03.000000 mglearn-0.1.9/mglearn/plot_pca.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1178 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_rbf_svm_parameters.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1017 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_ridge.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1505 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_scaling.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)      894 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plot_tree_nonmonotonous.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     3272 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/plots.py
--rw-rw-rw-   0 andy      (1000) andy      (1000)     4801 2020-05-25 21:15:34.000000 mglearn-0.1.9/mglearn/tools.py
-drwxrwxrwx   0 andy      (1000) andy      (1000)        0 2020-05-25 21:22:18.000000 mglearn-0.1.9/mglearn.egg-info/
--rw-rw-rw-   0 andy      (1000) andy      (1000)      365 2020-05-25 21:22:17.000000 mglearn-0.1.9/mglearn.egg-info/PKG-INFO
--rw-rw-rw-   0 andy      (1000) andy      (1000)     1077 2020-05-25 21:22:18.000000 mglearn-0.1.9/mglearn.egg-info/SOURCES.txt
--rw-rw-rw-   0 andy      (1000) andy      (1000)        1 2020-05-25 21:22:17.000000 mglearn-0.1.9/mglearn.egg-info/dependency_links.txt
--rw-rw-rw-   0 andy      (1000) andy      (1000)       66 2020-05-25 21:22:17.000000 mglearn-0.1.9/mglearn.egg-info/requires.txt
--rw-rw-rw-   0 andy      (1000) andy      (1000)        8 2020-05-25 21:22:17.000000 mglearn-0.1.9/mglearn.egg-info/top_level.txt
--rw-rw-rw-   0 andy      (1000) andy      (1000)       67 2020-05-25 21:22:18.000000 mglearn-0.1.9/setup.cfg
--rw-rw-rw-   0 andy      (1000) andy      (1000)      623 2020-05-25 21:21:42.000000 mglearn-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:43.468183 mglearn-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 02:38:28.000000 mglearn-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-01 02:38:43.468183 mglearn-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-01 02:38:28.000000 mglearn-0.2.0/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:43.456183 mglearn-0.2.0/mglearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:43.464183 mglearn-0.2.0/mglearn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3974305 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/data/adult.data
+-rw-r--r--   0 runner    (1001) docker     (123)   688092 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/data/citibike.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/data/ram_price.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_2d_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_agglomerative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_animal_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_improper_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_interactive_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_kneighbors_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_knn_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_knn_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_linear_svc_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_nn_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_rbf_svm_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plot_tree_nonmonotonous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-01 02:38:28.000000 mglearn-0.2.0/mglearn/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:43.460183 mglearn-0.2.0/mglearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-01 02:38:43.000000 mglearn-0.2.0/mglearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-01 02:38:43.000000 mglearn-0.2.0/mglearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:38:43.000000 mglearn-0.2.0/mglearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 02:38:43.000000 mglearn-0.2.0/mglearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 02:38:43.000000 mglearn-0.2.0/mglearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 02:38:43.468183 mglearn-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-01 02:38:28.000000 mglearn-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:38:43.468183 mglearn-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 02:38:28.000000 mglearn-0.2.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 02:38:28.000000 mglearn-0.2.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-01 02:38:28.000000 mglearn-0.2.0/tests/test_plot_2d_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-01 02:38:28.000000 mglearn-0.2.0/tests/test_plotting.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mglearn-0.1.9/Readme.md` & `mglearn-0.2.0/Readme.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 This repository is a stand-alone package in case you really feel like you want to
 install mglearn into your Python environment, for some reason or another. You can install it by running
 
     pip install mglearn
 
 in your terminal, or by running
 
-    !pip install mglearn
+    %pip install mglearn
 
 in Jupyter Notebook.
 
 In particular, installing this package is a very easy way to add it to your Python search path.
 Or you can just check out the notebooks from the repository above, and add the path to the
 mglearn subfolder to your PYTHONPATH environment variable (or set it in your IDE).
```

### Comparing `mglearn-0.1.9/mglearn/data/adult.data` & `mglearn-0.2.0/mglearn/data/adult.data`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/data/citibike.csv` & `mglearn-0.2.0/mglearn/data/citibike.csv`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/data/ram_price.csv` & `mglearn-0.2.0/mglearn/data/ram_price.csv`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_2d_separator.py` & `mglearn-0.2.0/mglearn/plot_2d_separator.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,18 +99,8 @@
         ax.contour(X1, X2, decision_values.reshape(X1.shape), levels=levels,
                    colors="black", alpha=alpha, linewidths=linewidth,
                    linestyles=linestyle, zorder=5)
 
     ax.set_xlim(x_min, x_max)
     ax.set_ylim(y_min, y_max)
     ax.set_xticks(())
-    ax.set_yticks(())
-
-
-if __name__ == '__main__':
-    from sklearn.datasets import make_blobs
-    from sklearn.linear_model import LogisticRegression
-    X, y = make_blobs(centers=2, random_state=42)
-    clf = LogisticRegression().fit(X, y)
-    plot_2d_separator(clf, X, fill=True)
-    discrete_scatter(X[:, 0], X[:, 1], y)
-    plt.show()
+    ax.set_yticks(())
```

### Comparing `mglearn-0.1.9/mglearn/plot_agglomerative.py` & `mglearn-0.2.0/mglearn/plot_agglomerative.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_animal_tree.py` & `mglearn-0.2.0/mglearn/plot_animal_tree.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_cross_validation.py` & `mglearn-0.2.0/mglearn/plot_cross_validation.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_dbscan.py` & `mglearn-0.2.0/mglearn/plot_dbscan.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_decomposition.py` & `mglearn-0.2.0/mglearn/plot_decomposition.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_grid_search.py` & `mglearn-0.2.0/mglearn/plot_grid_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,16 @@
                               alpha=.5)
         marker_mean, = plt.plot(i, row.mean_test_score, 'v', c='none', alpha=1,
                                 markersize=10, markeredgecolor='k')
         if i == best:
             marker_best, = plt.plot(i, row.mean_test_score, 'o', c='red',
                                     fillstyle="none", alpha=1, markersize=20,
                                     markeredgewidth=3)
-
     plt.xticks(range(len(results)), [str(x).strip("{}").replace("'", "") for x
-                                     in grid_search.cv_results_['params']],
+                                     in results['params']],
                rotation=90)
     plt.ylabel("Validation accuracy")
     plt.xlabel("Parameter settings")
     plt.legend([marker_cv, marker_mean, marker_best],
                ["cv accuracy", "mean accuracy", "best parameter setting"],
                loc=(1.05, .4))
```

### Comparing `mglearn-0.1.9/mglearn/plot_helpers.py` & `mglearn-0.2.0/mglearn/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_improper_preprocessing.py` & `mglearn-0.2.0/mglearn/plot_improper_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_interactive_tree.py` & `mglearn-0.2.0/mglearn/plot_interactive_tree.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_kmeans.py` & `mglearn-0.2.0/mglearn/plot_kmeans.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_kneighbors_regularization.py` & `mglearn-0.2.0/mglearn/plot_kneighbors_regularization.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,13 +18,8 @@
         kneighbor_regression = KNeighborsRegressor(n_neighbors=n_neighbors)
         kneighbor_regression.fit(X, y)
         ax.plot(x, y_no_noise, label="true function")
         ax.plot(x, y, "o", label="data")
         ax.plot(x_test, kneighbor_regression.predict(x_test[:, np.newaxis]),
                 label="prediction")
         ax.legend()
-        ax.set_title("n_neighbors = %d" % n_neighbors)
-
-
-if __name__ == "__main__":
-    plot_kneighbors_regularization()
-    plt.show()
+        ax.set_title("n_neighbors = %d" % n_neighbors)
```

### Comparing `mglearn-0.1.9/mglearn/plot_knn_classification.py` & `mglearn-0.2.0/mglearn/plot_knn_classification.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_knn_regression.py` & `mglearn-0.2.0/mglearn/plot_knn_regression.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_linear_regression.py` & `mglearn-0.2.0/mglearn/plot_linear_regression.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_linear_svc_regularization.py` & `mglearn-0.2.0/mglearn/plot_linear_svc_regularization.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,11 +27,7 @@
         ax.plot(xx, yy, c='k')
         ax.set_xlim(x_min, x_max)
         ax.set_ylim(y_min, y_max)
         ax.set_xticks(())
         ax.set_yticks(())
         ax.set_title("C = %f" % C)
     axes[0].legend(loc="best")
-
-if __name__ == "__main__":
-    plot_linear_svc_regularization()
-    plt.show()
```

### Comparing `mglearn-0.1.9/mglearn/plot_metrics.py` & `mglearn-0.2.0/mglearn/plot_metrics.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_nmf.py` & `mglearn-0.2.0/mglearn/plot_nmf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from sklearn.decomposition import NMF
 import matplotlib.pyplot as plt
 import numpy as np
 
 from joblib import Memory
 
-memory = Memory(cachedir="cache")
+try:
+    memory = Memory(cachedir="cache")
+except TypeError:
+    # joblib.Memory changed its API in 0.12
+    memory = Memory(location="cache", verbose=0)
 
 
 def plot_nmf_illustration():
     rnd = np.random.RandomState(5)
     X_ = rnd.normal(size=(300, 2))
     # Add 8 to make sure every point lies in the positive part of the space
     X_blob = np.dot(X_, rnd.normal(size=(2, 2))) + rnd.normal(size=2) + 8
```

### Comparing `mglearn-0.1.9/mglearn/plot_nn_graphs.py` & `mglearn-0.2.0/mglearn/plot_nn_graphs.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_pca.py` & `mglearn-0.2.0/mglearn/plot_pca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from sklearn.decomposition import PCA
 import matplotlib.pyplot as plt
 import numpy as np
 
 from joblib import Memory
 
-memory = Memory(cachedir="cache")
-
+try:
+    memory = Memory(cachedir="cache")
+except TypeError:
+    # joblib.Memory changed its API in 0.12
+    memory = Memory(location="cache", verbose=0)
 
 def plot_pca_illustration():
     rnd = np.random.RandomState(5)
     X_ = rnd.normal(size=(300, 2))
     X_blob = np.dot(X_, rnd.normal(size=(2, 2))) + rnd.normal(size=2)
 
     pca = PCA()
```

### Comparing `mglearn-0.1.9/mglearn/plot_rbf_svm_parameters.py` & `mglearn-0.2.0/mglearn/plot_rbf_svm_parameters.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_ridge.py` & `mglearn-0.2.0/mglearn/plot_ridge.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_scaling.py` & `mglearn-0.2.0/mglearn/plot_scaling.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plot_tree_nonmonotonous.py` & `mglearn-0.2.0/mglearn/plot_tree_nonmonotonous.py`

 * *Files identical despite different names*

### Comparing `mglearn-0.1.9/mglearn/plots.py` & `mglearn-0.2.0/mglearn/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from .plot_grid_search import plot_grid_search_overview, plot_cross_val_selection
 from .plot_metrics import (plot_confusion_matrix_illustration,
                            plot_binary_confusion_matrix,
                            plot_decision_threshold)
 from .plot_dbscan import plot_dbscan
 from .plot_ridge import plot_ridge_n_samples
+from .plot_kneighbors_regularization import plot_kneighbors_regularization
 
 __all__ = ['plot_linear_svc_regularization',
            "plot_animal_tree", "plot_tree_progressive",
            'plot_tree_partition', 'plot_svm',
            'plot_knn_regression',
            'plot_logistic_regression_graph',
            'plot_single_hidden_layer_graph',
@@ -61,9 +62,10 @@
            'plot_cross_validation',
            'plot_grid_search_overview',
            'plot_cross_val_selection',
            'plot_confusion_matrix_illustration',
            'plot_binary_confusion_matrix',
            'plot_decision_threshold',
            'plot_dbscan',
-           'plot_ridge_n_samples'
+           'plot_ridge_n_samples',
+           'plot_kneighbors_regularization'
            ]
```

### Comparing `mglearn-0.1.9/mglearn/tools.py` & `mglearn-0.2.0/mglearn/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     return img
 
 
 def make_handcrafted_dataset():
     # a carefully hand-designed dataset lol
     X, y = make_blobs(centers=2, random_state=4, n_samples=30)
     y[np.array([7, 27])] = 0
-    mask = np.ones(len(X), dtype=np.bool)
+    mask = np.ones(len(X), dtype=bool)
     mask[np.array([0, 1, 5, 26])] = 0
     X, y = X[mask], y[mask]
     return X, y
 
 
 def print_topics(topics, feature_names, sorting, topics_per_chunk=6,
                  n_words=20):
```

### Comparing `mglearn-0.1.9/mglearn.egg-info/SOURCES.txt` & `mglearn-0.2.0/mglearn.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 MANIFEST.in
 Readme.md
 setup.cfg
 setup.py
 mglearn/__init__.py
 mglearn/datasets.py
-mglearn/make_blobs.py
 mglearn/plot_2d_separator.py
 mglearn/plot_agglomerative.py
 mglearn/plot_animal_tree.py
 mglearn/plot_cross_validation.py
 mglearn/plot_dbscan.py
 mglearn/plot_decomposition.py
 mglearn/plot_grid_search.py
@@ -34,8 +33,12 @@
 mglearn.egg-info/PKG-INFO
 mglearn.egg-info/SOURCES.txt
 mglearn.egg-info/dependency_links.txt
 mglearn.egg-info/requires.txt
 mglearn.egg-info/top_level.txt
 mglearn/data/adult.data
 mglearn/data/citibike.csv
-mglearn/data/ram_price.csv
+mglearn/data/ram_price.csv
+tests/test_datasets.py
+tests/test_init.py
+tests/test_plot_2d_separator.py
+tests/test_plotting.py
```

### Comparing `mglearn-0.1.9/setup.py` & `mglearn-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mglearn",
-    version="0.1.9",
+    version="0.2.0",
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'scikit-learn', 'pandas',
                       'pillow', 'cycler', 'imageio', 'joblib'],
     include_package_data=True,
 
     author="Andreas Mueller",
     author_email="t3kcit@gmail.com",
     description=("Helper functions for the book "
-                 "'Introduction to machine learning with Python'"),
+                 "Introduction to machine learning with Python"),
+    long_description=("Helper functions for the book "
+                      "`Introduction to machine learning with Python`"),
+    long_description_content_type="text/markdown",
     license="BSD",
     keywords="machine learning ml sklearn scikit learn",
     url="https://github.com/amueller/introduction_to_ml_with_python",
 )
```

