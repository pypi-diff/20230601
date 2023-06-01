# Comparing `tmp/ipylgbst-0.2.0.tar.gz` & `tmp/ipylgbst-0.2.1.tar.gz`

## Comparing `ipylgbst-0.2.0.tar` & `ipylgbst-0.2.1.tar`

### file list

```diff
@@ -1,221 +1,70 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.eslintignore
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.prettierrc
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/babel.config.js
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/codecov.yml
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/install.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/jest.config.js
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/package.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/tsconfig.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/webpack.config.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/css/widget.css
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/environment.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/make.bat
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/develop-install.rst
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/introduction.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0    13508 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/introduction.ipynb
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/.jupyterlite.doit.db
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/bootstrap.js
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/config-utils.js
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/icon-120x120.png
--rw-r--r--   0        0        0    20954 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/icon-512x512.png
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/jupyter-lite.ipynb
--rw-r--r--   0        0        0     6568 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/jupyter-lite.json
--rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/jupyterlite.schema.v0.json
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/manifest.webmanifest
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/package.json
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/piplite.schema.v0.json
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/service-worker-b2fb40a.js
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/api/contents/all.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/api/translations/all.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/api/translations/en.json
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/doc/workspaces/index.html
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/install.json
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/package.json
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/1.6c3ab69171002cbfa04f.js
--rw-r--r--   0        0        0   154302 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/113.dd66397047ecb9a605cf.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/113.dd66397047ecb9a605cf.js.LICENSE.txt
--rw-r--r--   0        0        0    85597 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/134.40eaa5b8e976096d50b2.js
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/150.b0e841b75317744a7595.js
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/18.c756b86bf6ebd74dab7b.js
--rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/243.6c384ff2649ef572a18a.js
--rw-r--r--   0        0        0    39969 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/272.3fcd6d7045eecfb56da6.js
--rw-r--r--   0        0        0    18420 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/279.aa88a78c8bf62c65db54.js
--rw-r--r--   0        0        0    90076 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/291.f707f721e4b3a5489ee0.js
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/291.f707f721e4b3a5489ee0.js.LICENSE.txt
--rw-r--r--   0        0        0    38441 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/345.03be96cd091aac4797a5.js
--rw-r--r--   0        0        0   111538 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/466.f77b3df99f049604bce9.js
--rw-r--r--   0        0        0   111264 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/495.5805e8bf9dd8851289a1.js
--rw-r--r--   0        0        0    53936 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/523.66fca84c7924f6f7676d.js
--rw-r--r--   0        0        0    23918 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/595.e3c9c115ecf5763f080b.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/596.5d35bd634ac768ff6d16.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/61.21f571face17e35076c2.js
--rw-r--r--   0        0        0    88696 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/638.f3e5e34a28f3334d4f08.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/638.f3e5e34a28f3334d4f08.js.LICENSE.txt
--rw-r--r--   0        0        0    57036 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/644.11f638668109f1562dd1.js
--rw-r--r--   0        0        0    32641 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/699.563670613eea7b633a22.js
--rw-r--r--   0        0        0    37904 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/803.b7b75bd6e7977a648c67.js
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/86.970ef07abcc86672015c.js
--rw-r--r--   0        0        0    27436 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/95.b5a5ff10000a6051fa99.js
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/95.b5a5ff10000a6051fa99.js.LICENSE.txt
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/965.7ea93aa594250a988d2a.js
--rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/remoteEntry.1bd01b57743def902f73.js
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/remoteEntry.d6df56cd69f4640706bc.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/style.js
--rw-r--r--   0        0        0    36297 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/install.json
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/package.json
--rw-r--r--   0        0        0    15607 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/133.2df0d387bef0b99e239a.js
--rw-r--r--   0        0        0   538309 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/212.898d3b3da016aa77edc1.js
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/212.898d3b3da016aa77edc1.js.LICENSE.txt
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/501.6c13f92ce49688bde790.js
--rw-r--r--   0        0        0   422624 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/568.829152b9fd5d5b1dc823.js
--rw-r--r--   0        0        0   200722 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/662.d928d9e888427c5996be.js
--rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/794.8d6261fd8a7307e156f7.js
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/815.4fcd9a1489787115f930.js
--rw-r--r--   0        0        0    54310 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/842.a94bbf6f3349e982fb8b.js
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/87.cc5d175e0ffc0d125bd5.js
--rw-r--r--   0        0        0    20892 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/981.3f93685e278b785a3338.js
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/981.3f93685e278b785a3338.js.LICENSE.txt
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/remoteEntry.99c828c2ee313756f7dc.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/style.js
--rw-r--r--   0        0        0    64818 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/static/third-party-licenses.json
--rw-r--r--   0        0        0    20729 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/build_log.json
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/package.json
--rw-r--r--   0        0        0   148280 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lego-boost-browser_dist_legoBoost_js.efb9a5c4ab34d7609900.js
--rw-r--r--   0        0        0   173367 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lego-boost-browser_dist_legoBoost_js.efb9a5c4ab34d7609900.js.map
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lego-boost-browser_node_modules_ieee754_index_js.b881643aeb45daabb9e9.js
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lego-boost-browser_node_modules_ieee754_index_js.b881643aeb45daabb9e9.js.map
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_index_js.747fd85bc4f1428909e5.js
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_index_js.747fd85bc4f1428909e5.js.map
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_plugin_js.ffb1de07b5e860a813b2.js
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_plugin_js.ffb1de07b5e860a813b2.js.map
--rw-r--r--   0        0        0    29848 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_widget_js.29800352127817c035b1.js
--rw-r--r--   0        0        0    30685 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_widget_js.29800352127817c035b1.js.map
--rw-r--r--   0        0        0    29782 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_widget_js.58bf2d37e47496e149e9.js
--rw-r--r--   0        0        0    30483 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_widget_js.58bf2d37e47496e149e9.js.map
--rw-r--r--   0        0        0    29963 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_widget_js.ae8f97344fd0144a9bc7.js
--rw-r--r--   0        0        0    30682 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/lib_widget_js.ae8f97344fd0144a9bc7.js.map
--rw-r--r--   0        0        0    27969 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/remoteEntry.7498176bc923abab92a5.js
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/remoteEntry.7498176bc923abab92a5.js.map
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/remoteEntry.d7fe2150d0862916b497.js.map
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/remoteEntry.ec151e601f43b2ce7a40.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/ipylgbst/static/style.js
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/install.json
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/package.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/extensions/jupyterlab_pygments/static/third-party-licenses.json
--rw-r--r--   0        0        0    13508 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/files/introduction.ipynb
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/kernelspecs/javascript.svg
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/kernelspecs/python.svg
--rw-r--r--   0        0        0   324251 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/favicon.ico
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/jupyter-lite.ipynb
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/jupyter-lite.json
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/package.json
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/tree/index.html
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/lab/workspaces/index.html
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/repl/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/repl/jupyter-lite.ipynb
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/repl/jupyter-lite.json
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/repl/package.json
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/favicon.ico
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/jupyter-lite.ipynb
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/jupyter-lite.json
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/package.json
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/consoles/favicon.ico
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/consoles/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/consoles/jupyter-lite.ipynb
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/consoles/jupyter-lite.json
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/edit/favicon.ico
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/edit/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/edit/jupyter-lite.ipynb
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/edit/jupyter-lite.json
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/notebooks/favicon.ico
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/notebooks/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/notebooks/jupyter-lite.ipynb
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/notebooks/jupyter-lite.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/tree/index.html
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/tree/jupyter-lite.ipynb
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/retro/tree/jupyter-lite.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/examples/lite/_output/tree/index.html
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/_frontend.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/_version.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/lego_boost.py
--rw-r--r--   0        0        0    20729 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/build_log.json
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/package.json
--rw-r--r--   0        0        0   148280 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lego-boost-browser_dist_legoBoost_js.efb9a5c4ab34d7609900.js
--rw-r--r--   0        0        0   173367 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lego-boost-browser_dist_legoBoost_js.efb9a5c4ab34d7609900.js.map
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lego-boost-browser_node_modules_ieee754_index_js.b881643aeb45daabb9e9.js
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lego-boost-browser_node_modules_ieee754_index_js.b881643aeb45daabb9e9.js.map
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_index_js.747fd85bc4f1428909e5.js
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_index_js.747fd85bc4f1428909e5.js.map
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_plugin_js.ffb1de07b5e860a813b2.js
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_plugin_js.ffb1de07b5e860a813b2.js.map
--rw-r--r--   0        0        0    29848 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.29800352127817c035b1.js
--rw-r--r--   0        0        0    30685 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.29800352127817c035b1.js.map
--rw-r--r--   0        0        0    29782 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.58bf2d37e47496e149e9.js
--rw-r--r--   0        0        0    30483 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.58bf2d37e47496e149e9.js.map
--rw-r--r--   0        0        0    29963 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.ae8f97344fd0144a9bc7.js
--rw-r--r--   0        0        0    30682 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.ae8f97344fd0144a9bc7.js.map
--rw-r--r--   0        0        0    29782 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.af2549312e969079e0e6.js
--rw-r--r--   0        0        0    30483 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/lib_widget_js.af2549312e969079e0e6.js.map
--rw-r--r--   0        0        0    27969 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/remoteEntry.3b2abbae90ab34fc6ce9.js
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/remoteEntry.3b2abbae90ab34fc6ce9.js.map
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/remoteEntry.7498176bc923abab92a5.js.map
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/remoteEntry.d7fe2150d0862916b497.js.map
--rw-r--r--   0        0        0    26717 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/remoteEntry.ec151e601f43b2ce7a40.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/labextension/static/style.js
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/nbextension/extension.js
--rw-r--r--   0        0        0   184404 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/nbextension/index.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0   245406 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/tests/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/tests/conftest.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/ipylgbst/tests/test_widget.py
--rw-r--r--   0        0        0   340513 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/pydist/ipylgbst-0.1.3-py3-none-any.whl
--rw-r--r--   0        0        0   595585 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/pydist/ipylgbst-0.1.3.tar.gz
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/extension.ts
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/plugin.ts
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/version.ts
--rw-r--r--   0        0        0    11087 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/widget.ts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/README.md
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 ipylgbst-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.eslintignore
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.prettierrc
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/babel.config.js
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/codecov.yml
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/install.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/jest.config.js
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/package.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/webpack.config.js
+-rw-r--r--   0        0        0   320557 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/yarn.lock
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/css/widget.css
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/environment.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/introduction.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/_frontend.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/_version.py
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/lego_boost.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/package.json
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/367.74c161ae4e86a0b029fa.js
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/480.111fe52b0bb8bef2b483.js
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/568.9e40f9ba6cbae7c31be3.js
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/645.674af9133fa659e9cf20.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/645.674af9133fa659e9cf20.js.LICENSE.txt
+-rw-r--r--   0        0        0    53528 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/969.1fd936b9612eb398d454.js
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/969.1fd936b9612eb398d454.js.LICENSE.txt
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/remoteEntry.b09d97918120529e3908.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/style.js
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/nbextension/extension.js
+-rw-r--r--   0        0        0    71137 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/nbextension/index.js
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0   214169 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/tests/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/tests/conftest.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/ipylgbst/tests/test_widget.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/extension.ts
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/plugin.ts
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/version.ts
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/widget.ts
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/README.md
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 ipylgbst-0.2.1/PKG-INFO
```

### Comparing `ipylgbst-0.2.0/.eslintrc.js` & `ipylgbst-0.2.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/MANIFEST.in` & `ipylgbst-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/package.json` & `ipylgbst-0.2.1/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8965564503932244%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/jupyterlab-contrib-ipylgbst/issues'}",*

 * * "'dependencies'": "{'@lumino/application': '^1.6.0', '@lumino/widgets': '^1.6.0'}",*

 * * "'devDependencies'": "{delete: ['@lumino/application', '@lumino/widgets']}",*

 * * "'homepage'": "'https://github.com/jupyterlab-contrib-ipylgbst'",*

 * * "'repository'": "{'url': 'https://github.com/jupyterlab-contrib-ipylgbst'}",*

 * * "'scripts'": "{'build': 'jlpm run build:lib && jlpm run build:nbextension && jlpm run "*

 * *              "build:labextension:de […]*

```diff
@@ -1,29 +1,29 @@
 {
     "author": {
         "email": "derthorstenbeier@gmail.com",
         "name": "Thorsten Beier"
     },
     "bugs": {
-        "url": "https://github.com/DerThorsten/ipylgbst/issues"
+        "url": "https://github.com/jupyterlab-contrib-ipylgbst/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6",
+        "@lumino/application": "^1.6.0",
+        "@lumino/widgets": "^1.6.0",
         "add": "^2.0.6",
         "ieee754": "^1.2.1",
         "lego-boost-browser": "git+https://github.com/DerThorsten/lego-boost-browser.git"
     },
     "description": "A widget library for controlling LEGO\u00ae BOOST via web-bluetooth",
     "devDependencies": {
         "@babel/core": "^7.5.0",
         "@babel/preset-env": "^7.5.0",
         "@jupyter-widgets/base-manager": "^1.0.2",
         "@jupyterlab/builder": "^3.0.0",
-        "@lumino/application": "^1.6.0",
-        "@lumino/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
         "eslint": "^7.4.0",
@@ -45,15 +45,15 @@
         "webpack-cli": "^4.0.0"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
-    "homepage": "https://github.com/DerThorsten/ipylgbst",
+    "homepage": "https://github.com/jupyterlab-contrib-ipylgbst",
     "jupyterlab": {
         "extension": "lib/plugin",
         "outputDir": "ipylgbst/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -67,32 +67,33 @@
         "widgets"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "ipylgbst",
     "repository": {
         "type": "git",
-        "url": "https://github.com/DerThorsten/ipylgbst"
+        "url": "https://github.com/jupyterlab-contrib-ipylgbst"
     },
     "scripts": {
-        "build": "yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev",
+        "build": "jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:nbextension": "webpack",
-        "build:prod": "yarn run build:lib && yarn run build:nbextension && yarn run build:labextension",
-        "clean": "yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension",
+        "build:prod": "jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension",
+        "clean": "jlpm run clean:lib && jlpm run clean:nbextension && jlpm run clean:labextension",
         "clean:labextension": "rimraf ipylgbst/labextension",
         "clean:lib": "rimraf lib",
         "clean:nbextension": "rimraf ipylgbst/nbextension/static/index.js",
+        "install:extension": "jlpm build",
         "lint": "eslint . --ext .ts,.tsx --fix",
         "lint:check": "eslint . --ext .ts,.tsx",
-        "prepack": "yarn run build:lib",
+        "prepack": "jlpm run build:lib",
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `ipylgbst-0.2.0/tsconfig.json` & `ipylgbst-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/webpack.config.js` & `ipylgbst-0.2.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/docs/Makefile` & `ipylgbst-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/docs/make.bat` & `ipylgbst-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/docs/source/conf.py` & `ipylgbst-0.2.1/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,25 +67,32 @@
 # built documents.
 #
 # The short X.Y version.
 
 
 # get version from python package:
 import os
+import json
 here = os.path.dirname(__file__)
 repo = os.path.join(here, '..', '..')
-_version_py = os.path.join(repo, 'ipylgbst', '_version.py')
-version_ns = {}
-with open(_version_py) as f:
-    exec(f.read(), version_ns)
+package_json = os.path.join(repo, 'package.json')
+
+data = {}
+with open(package_json) as f:
+    data = json.load(f)
+
+#_version_py = os.path.join(repo, 'ipylgbst', '_version.py')
+#version_ns = {}
+#with open(_version_py) as f:
+#    exec(f.read(), version_ns)
 
 # The short X.Y version.
-version = '%i.%i' % version_ns['version_info'][:2]
+version = '%s.%s' % (data["version"][0], data["version"][2])
 # The full version, including alpha/beta/rc tags.
-release = version_ns['__version__']
+release = data["version"]
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `ipylgbst-0.2.0/docs/source/develop-install.rst` & `ipylgbst-0.2.1/docs/source/develop-install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Developer install
 =================
 
 
 To install a developer version of ipylgbst, you will first need to clone
 the repository::
 
-    git clone https://github.com/DerThorsten/ipylgbst
+    git clone https://github.com/jupyterlab-contrib-ipylgbst
     cd ipylgbst
 
 Next, install it with a develop install using pip::
 
     pip install -e .
```

### Comparing `ipylgbst-0.2.0/docs/source/index.rst` & `ipylgbst-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/docs/source/installing.rst` & `ipylgbst-0.2.1/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/examples/lite/_output/extensions/@jupyter-widgets/jupyterlab-manager/static/644.11f638668109f1562dd1.js` & `ipylgbst-0.2.1/ipylgbst/labextension/static/969.1fd936b9612eb398d454.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,2939 +1,2101 @@
-(self.webpackChunk_jupyter_widgets_jupyterlab_manager = self.webpackChunk_jupyter_widgets_jupyterlab_manager || []).push([
-    [644], {
-        7298: (t, e, r) => {
-            var n, i, o;
-            o = "object" == typeof self && self.self === self && self || "object" == typeof r.g && r.g.global === r.g && r.g, n = [r(3506), r(8830), e], i = function(t, e, r) {
-                o.Backbone = function(t, e, r, n) {
-                    var i = t.Backbone,
-                        o = Array.prototype.slice;
-                    e.VERSION = "1.4.0", e.$ = n, e.noConflict = function() {
-                        return t.Backbone = i, this
-                    }, e.emulateHTTP = !1, e.emulateJSON = !1;
-                    var s, a = e.Events = {},
-                        u = /\s+/,
-                        c = function(t, e, n, i, o) {
-                            var s, a = 0;
-                            if (n && "object" == typeof n) {
-                                void 0 !== i && "context" in o && void 0 === o.context && (o.context = i);
-                                for (s = r.keys(n); a < s.length; a++) e = c(t, e, s[a], n[s[a]], o)
-                            } else if (n && u.test(n))
-                                for (s = n.split(u); a < s.length; a++) e = t(e, s[a], i, o);
-                            else e = t(e, n, i, o);
-                            return e
-                        };
-                    a.on = function(t, e, r) {
-                        return this._events = c(l, this._events || {}, t, e, {
-                            context: r,
-                            ctx: this,
-                            listening: s
-                        }), s && ((this._listeners || (this._listeners = {}))[s.id] = s, s.interop = !1), this
-                    }, a.listenTo = function(t, e, n) {
-                        if (!t) return this;
-                        var i = t._listenId || (t._listenId = r.uniqueId("l")),
-                            o = this._listeningTo || (this._listeningTo = {}),
-                            a = s = o[i];
-                        a || (this._listenId || (this._listenId = r.uniqueId("l")), a = s = o[i] = new g(this, t));
-                        var u = h(t, e, n, this);
-                        if (s = void 0, u) throw u;
-                        return a.interop && a.on(e, n), this
-                    };
-                    var l = function(t, e, r, n) {
-                            if (r) {
-                                var i = t[e] || (t[e] = []),
-                                    o = n.context,
-                                    s = n.ctx,
-                                    a = n.listening;
-                                a && a.count++, i.push({
-                                    callback: r,
-                                    context: o,
-                                    ctx: o || s,
-                                    listening: a
-                                })
-                            }
-                            return t
-                        },
-                        h = function(t, e, r, n) {
+/*! For license information please see 969.1fd936b9612eb398d454.js.LICENSE.txt */
+"use strict";
+(self.webpackChunkipylgbst = self.webpackChunkipylgbst || []).push([
+    [969], {
+        742: (t, e) => {
+            e.byteLength = function(t) {
+                var e = s(t),
+                    r = e[0],
+                    n = e[1];
+                return 3 * (r + n) / 4 - n
+            }, e.toByteArray = function(t) {
+                var e, r, o = s(t),
+                    u = o[0],
+                    c = o[1],
+                    a = new i(function(t, e, r) {
+                        return 3 * (e + r) / 4 - r
+                    }(0, u, c)),
+                    f = 0,
+                    h = c > 0 ? u - 4 : u;
+                for (r = 0; r < h; r += 4) e = n[t.charCodeAt(r)] << 18 | n[t.charCodeAt(r + 1)] << 12 | n[t.charCodeAt(r + 2)] << 6 | n[t.charCodeAt(r + 3)], a[f++] = e >> 16 & 255, a[f++] = e >> 8 & 255, a[f++] = 255 & e;
+                return 2 === c && (e = n[t.charCodeAt(r)] << 2 | n[t.charCodeAt(r + 1)] >> 4, a[f++] = 255 & e), 1 === c && (e = n[t.charCodeAt(r)] << 10 | n[t.charCodeAt(r + 1)] << 4 | n[t.charCodeAt(r + 2)] >> 2, a[f++] = e >> 8 & 255, a[f++] = 255 & e), a
+            }, e.fromByteArray = function(t) {
+                for (var e, n = t.length, i = n % 3, o = [], u = 16383, s = 0, a = n - i; s < a; s += u) o.push(c(t, s, s + u > a ? a : s + u));
+                return 1 === i ? (e = t[n - 1], o.push(r[e >> 2] + r[e << 4 & 63] + "==")) : 2 === i && (e = (t[n - 2] << 8) + t[n - 1], o.push(r[e >> 10] + r[e >> 4 & 63] + r[e << 2 & 63] + "=")), o.join("")
+            };
+            for (var r = [], n = [], i = "undefined" != typeof Uint8Array ? Uint8Array : Array, o = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", u = 0; u < 64; ++u) r[u] = o[u], n[o.charCodeAt(u)] = u;
+
+            function s(t) {
+                var e = t.length;
+                if (e % 4 > 0) throw new Error("Invalid string. Length must be a multiple of 4");
+                var r = t.indexOf("=");
+                return -1 === r && (r = e), [r, r === e ? 0 : 4 - r % 4]
+            }
+
+            function c(t, e, n) {
+                for (var i, o, u = [], s = e; s < n; s += 3) i = (t[s] << 16 & 16711680) + (t[s + 1] << 8 & 65280) + (255 & t[s + 2]), u.push(r[(o = i) >> 18 & 63] + r[o >> 12 & 63] + r[o >> 6 & 63] + r[63 & o]);
+                return u.join("")
+            }
+            n["-".charCodeAt(0)] = 62, n["_".charCodeAt(0)] = 63
+        },
+        14: function(t, e, r) {
+            var n = this && this.__assign || function() {
+                    return n = Object.assign || function(t) {
+                        for (var e, r = 1, n = arguments.length; r < n; r++)
+                            for (var i in e = arguments[r]) Object.prototype.hasOwnProperty.call(e, i) && (t[i] = e[i]);
+                        return t
+                    }, n.apply(this, arguments)
+                },
+                i = this && this.__awaiter || function(t, e, r, n) {
+                    return new(r || (r = Promise))((function(i, o) {
+                        function u(t) {
                             try {
-                                t.on(e, r, n)
+                                c(n.next(t))
                             } catch (t) {
-                                return t
+                                o(t)
                             }
-                        };
-                    a.off = function(t, e, r) {
-                        return this._events ? (this._events = c(f, this._events, t, e, {
-                            context: r,
-                            listeners: this._listeners
-                        }), this) : this
-                    }, a.stopListening = function(t, e, n) {
-                        var i = this._listeningTo;
-                        if (!i) return this;
-                        for (var o = t ? [t._listenId] : r.keys(i), s = 0; s < o.length; s++) {
-                            var a = i[o[s]];
-                            if (!a) break;
-                            a.obj.off(e, n, this), a.interop && a.off(e, n)
                         }
-                        return r.isEmpty(i) && (this._listeningTo = void 0), this
-                    };
-                    var f = function(t, e, n, i) {
-                        if (t) {
-                            var o, s = i.context,
-                                a = i.listeners,
-                                u = 0;
-                            if (e || s || n) {
-                                for (o = e ? [e] : r.keys(t); u < o.length; u++) {
-                                    var c = t[e = o[u]];
-                                    if (!c) break;
-                                    for (var l = [], h = 0; h < c.length; h++) {
-                                        var f = c[h];
-                                        if (n && n !== f.callback && n !== f.callback._callback || s && s !== f.context) l.push(f);
-                                        else {
-                                            var p = f.listening;
-                                            p && p.off(e, n)
-                                        }
-                                    }
-                                    l.length ? t[e] = l : delete t[e]
-                                }
-                                return t
+
+                        function s(t) {
+                            try {
+                                c(n.throw(t))
+                            } catch (t) {
+                                o(t)
                             }
-                            for (o = r.keys(a); u < o.length; u++) a[o[u]].cleanup()
                         }
-                    };
-                    a.once = function(t, e, r) {
-                        var n = c(p, {}, t, e, this.off.bind(this));
-                        return "string" == typeof t && null == r && (e = void 0), this.on(n, e, r)
-                    }, a.listenToOnce = function(t, e, r) {
-                        var n = c(p, {}, e, r, this.stopListening.bind(this, t));
-                        return this.listenTo(t, n)
-                    };
-                    var p = function(t, e, n, i) {
-                        if (n) {
-                            var o = t[e] = r.once((function() {
-                                i(e, o), n.apply(this, arguments)
-                            }));
-                            o._callback = n
+
+                        function c(t) {
+                            var e;
+                            t.done ? i(t.value) : (e = t.value, e instanceof r ? e : new r((function(t) {
+                                t(e)
+                            }))).then(u, s)
                         }
-                        return t
-                    };
-                    a.trigger = function(t) {
-                        if (!this._events) return this;
-                        for (var e = Math.max(0, arguments.length - 1), r = Array(e), n = 0; n < e; n++) r[n] = arguments[n + 1];
-                        return c(d, this._events, t, void 0, r), this
-                    };
-                    var d = function(t, e, r, n) {
-                            if (t) {
-                                var i = t[e],
-                                    o = t.all;
-                                i && o && (o = o.slice()), i && v(i, n), o && v(o, [e].concat(n))
-                            }
-                            return t
-                        },
-                        v = function(t, e) {
-                            var r, n = -1,
-                                i = t.length,
-                                o = e[0],
-                                s = e[1],
-                                a = e[2];
-                            switch (e.length) {
-                                case 0:
-                                    for (; ++n < i;)(r = t[n]).callback.call(r.ctx);
-                                    return;
-                                case 1:
-                                    for (; ++n < i;)(r = t[n]).callback.call(r.ctx, o);
-                                    return;
-                                case 2:
-                                    for (; ++n < i;)(r = t[n]).callback.call(r.ctx, o, s);
-                                    return;
-                                case 3:
-                                    for (; ++n < i;)(r = t[n]).callback.call(r.ctx, o, s, a);
-                                    return;
-                                default:
-                                    for (; ++n < i;)(r = t[n]).callback.apply(r.ctx, e);
-                                    return
-                            }
+                        c((n = n.apply(t, e || [])).next())
+                    }))
+                },
+                o = this && this.__generator || function(t, e) {
+                    var r, n, i, o, u = {
+                        label: 0,
+                        sent: function() {
+                            if (1 & i[0]) throw i[1];
+                            return i[1]
                         },
-                        g = function(t, e) {
-                            this.id = t._listenId, this.listener = t, this.obj = e, this.interop = !0, this.count = 0, this._events = void 0
-                        };
-                    g.prototype.on = a.on, g.prototype.off = function(t, e) {
-                        var r;
-                        this.interop ? (this._events = c(f, this._events, t, e, {
-                            context: void 0,
-                            listeners: void 0
-                        }), r = !this._events) : (this.count--, r = 0 === this.count), r && this.cleanup()
-                    }, g.prototype.cleanup = function() {
-                        delete this.listener._listeningTo[this.obj._listenId], this.interop || delete this.obj._listeners[this.id]
-                    }, a.bind = a.on, a.unbind = a.off, r.extend(e, a);
-                    var y = e.Model = function(t, e) {
-                        var n = t || {};
-                        e || (e = {}), this.preinitialize.apply(this, arguments), this.cid = r.uniqueId(this.cidPrefix), this.attributes = {}, e.collection && (this.collection = e.collection), e.parse && (n = this.parse(n, e) || {});
-                        var i = r.result(this, "defaults");
-                        n = r.defaults(r.extend({}, i, n), i), this.set(n, e), this.changed = {}, this.initialize.apply(this, arguments)
+                        trys: [],
+                        ops: []
                     };
-                    r.extend(y.prototype, a, {
-                        changed: null,
-                        validationError: null,
-                        idAttribute: "id",
-                        cidPrefix: "c",
-                        preinitialize: function() {},
-                        initialize: function() {},
-                        toJSON: function(t) {
-                            return r.clone(this.attributes)
-                        },
-                        sync: function() {
-                            return e.sync.apply(this, arguments)
-                        },
-                        get: function(t) {
-                            return this.attributes[t]
-                        },
-                        escape: function(t) {
-                            return r.escape(this.get(t))
-                        },
-                        has: function(t) {
-                            return null != this.get(t)
-                        },
-                        matches: function(t) {
-                            return !!r.iteratee(t, this)(this.attributes)
-                        },
-                        set: function(t, e, n) {
-                            if (null == t) return this;
-                            var i;
-                            if ("object" == typeof t ? (i = t, n = e) : (i = {})[t] = e, n || (n = {}), !this._validate(i, n)) return !1;
-                            var o = n.unset,
-                                s = n.silent,
-                                a = [],
-                                u = this._changing;
-                            this._changing = !0, u || (this._previousAttributes = r.clone(this.attributes), this.changed = {});
-                            var c = this.attributes,
-                                l = this.changed,
-                                h = this._previousAttributes;
-                            for (var f in i) e = i[f], r.isEqual(c[f], e) || a.push(f), r.isEqual(h[f], e) ? delete l[f] : l[f] = e, o ? delete c[f] : c[f] = e;
-                            if (this.idAttribute in i && (this.id = this.get(this.idAttribute)), !s) {
-                                a.length && (this._pending = n);
-                                for (var p = 0; p < a.length; p++) this.trigger("change:" + a[p], this, c[a[p]], n)
-                            }
-                            if (u) return this;
-                            if (!s)
-                                for (; this._pending;) n = this._pending, this._pending = !1, this.trigger("change", this, n);
-                            return this._pending = !1, this._changing = !1, this
-                        },
-                        unset: function(t, e) {
-                            return this.set(t, void 0, r.extend({}, e, {
-                                unset: !0
-                            }))
-                        },
-                        clear: function(t) {
-                            var e = {};
-                            for (var n in this.attributes) e[n] = void 0;
-                            return this.set(e, r.extend({}, t, {
-                                unset: !0
-                            }))
-                        },
-                        hasChanged: function(t) {
-                            return null == t ? !r.isEmpty(this.changed) : r.has(this.changed, t)
-                        },
-                        changedAttributes: function(t) {
-                            if (!t) return !!this.hasChanged() && r.clone(this.changed);
-                            var e, n = this._changing ? this._previousAttributes : this.attributes,
-                                i = {};
-                            for (var o in t) {
-                                var s = t[o];
-                                r.isEqual(n[o], s) || (i[o] = s, e = !0)
-                            }
-                            return !!e && i
-                        },
-                        previous: function(t) {
-                            return null != t && this._previousAttributes ? this._previousAttributes[t] : null
-                        },
-                        previousAttributes: function() {
-                            return r.clone(this._previousAttributes)
-                        },
-                        fetch: function(t) {
-                            t = r.extend({
-                                parse: !0
-                            }, t);
-                            var e = this,
-                                n = t.success;
-                            return t.success = function(r) {
-                                var i = t.parse ? e.parse(r, t) : r;
-                                if (!e.set(i, t)) return !1;
-                                n && n.call(t.context, e, r, t), e.trigger("sync", e, r, t)
-                            }, q(this, t), this.sync("read", this, t)
-                        },
-                        save: function(t, e, n) {
-                            var i;
-                            null == t || "object" == typeof t ? (i = t, n = e) : (i = {})[t] = e;
-                            var o = (n = r.extend({
-                                validate: !0,
-                                parse: !0
-                            }, n)).wait;
-                            if (i && !o) {
-                                if (!this.set(i, n)) return !1
-                            } else if (!this._validate(i, n)) return !1;
-                            var s = this,
-                                a = n.success,
-                                u = this.attributes;
-                            n.success = function(t) {
-                                s.attributes = u;
-                                var e = n.parse ? s.parse(t, n) : t;
-                                if (o && (e = r.extend({}, i, e)), e && !s.set(e, n)) return !1;
-                                a && a.call(n.context, s, t, n), s.trigger("sync", s, t, n)
-                            }, q(this, n), i && o && (this.attributes = r.extend({}, u, i));
-                            var c = this.isNew() ? "create" : n.patch ? "patch" : "update";
-                            "patch" !== c || n.attrs || (n.attrs = i);
-                            var l = this.sync(c, this, n);
-                            return this.attributes = u, l
-                        },
-                        destroy: function(t) {
-                            t = t ? r.clone(t) : {};
-                            var e = this,
-                                n = t.success,
-                                i = t.wait,
-                                o = function() {
-                                    e.stopListening(), e.trigger("destroy", e, e.collection, t)
-                                };
-                            t.success = function(r) {
-                                i && o(), n && n.call(t.context, e, r, t), e.isNew() || e.trigger("sync", e, r, t)
-                            };
-                            var s = !1;
-                            return this.isNew() ? r.defer(t.success) : (q(this, t), s = this.sync("delete", this, t)), i || o(), s
-                        },
-                        url: function() {
-                            var t = r.result(this, "urlRoot") || r.result(this.collection, "url") || L();
-                            if (this.isNew()) return t;
-                            var e = this.get(this.idAttribute);
-                            return t.replace(/[^\/]$/, "$&/") + encodeURIComponent(e)
-                        },
-                        parse: function(t, e) {
-                            return t
-                        },
-                        clone: function() {
-                            return new this.constructor(this.attributes)
-                        },
-                        isNew: function() {
-                            return !this.has(this.idAttribute)
-                        },
-                        isValid: function(t) {
-                            return this._validate({}, r.extend({}, t, {
-                                validate: !0
-                            }))
-                        },
-                        _validate: function(t, e) {
-                            if (!e.validate || !this.validate) return !0;
-                            t = r.extend({}, this.attributes, t);
-                            var n = this.validationError = this.validate(t, e) || null;
-                            return !n || (this.trigger("invalid", this, n, r.extend(e, {
-                                validationError: n
-                            })), !1)
-                        }
-                    });
-                    var _ = e.Collection = function(t, e) {
-                            e || (e = {}), this.preinitialize.apply(this, arguments), e.model && (this.model = e.model), void 0 !== e.comparator && (this.comparator = e.comparator), this._reset(), this.initialize.apply(this, arguments), t && this.reset(t, r.extend({
-                                silent: !0
-                            }, e))
-                        },
-                        b = {
-                            add: !0,
-                            remove: !0,
-                            merge: !0
-                        },
-                        m = {
-                            add: !0,
-                            remove: !1
-                        },
-                        x = function(t, e, r) {
-                            r = Math.min(Math.max(r, 0), t.length);
-                            var n, i = Array(t.length - r),
-                                o = e.length;
-                            for (n = 0; n < i.length; n++) i[n] = t[n + r];
-                            for (n = 0; n < o; n++) t[n + r] = e[n];
-                            for (n = 0; n < i.length; n++) t[n + o + r] = i[n]
-                        };
-                    r.extend(_.prototype, a, {
-                        model: y,
-                        preinitialize: function() {},
-                        initialize: function() {},
-                        toJSON: function(t) {
-                            return this.map((function(e) {
-                                return e.toJSON(t)
-                            }))
-                        },
-                        sync: function() {
-                            return e.sync.apply(this, arguments)
-                        },
-                        add: function(t, e) {
-                            return this.set(t, r.extend({
-                                merge: !1
-                            }, e, m))
-                        },
-                        remove: function(t, e) {
-                            e = r.extend({}, e);
-                            var n = !r.isArray(t);
-                            t = n ? [t] : t.slice();
-                            var i = this._removeModels(t, e);
-                            return !e.silent && i.length && (e.changes = {
-                                added: [],
-                                merged: [],
-                                removed: i
-                            }, this.trigger("update", this, e)), n ? i[0] : i
-                        },
-                        set: function(t, e) {
-                            if (null != t) {
-                                (e = r.extend({}, b, e)).parse && !this._isModel(t) && (t = this.parse(t, e) || []);
-                                var n = !r.isArray(t);
-                                t = n ? [t] : t.slice();
-                                var i = e.at;
-                                null != i && (i = +i), i > this.length && (i = this.length), i < 0 && (i += this.length + 1);
-                                var o, s, a = [],
-                                    u = [],
-                                    c = [],
-                                    l = [],
-                                    h = {},
-                                    f = e.add,
-                                    p = e.merge,
-                                    d = e.remove,
-                                    v = !1,
-                                    g = this.comparator && null == i && !1 !== e.sort,
-                                    y = r.isString(this.comparator) ? this.comparator : null;
-                                for (s = 0; s < t.length; s++) {
-                                    o = t[s];
-                                    var _ = this.get(o);
-                                    if (_) {
-                                        if (p && o !== _) {
-                                            var m = this._isModel(o) ? o.attributes : o;
-                                            e.parse && (m = _.parse(m, e)), _.set(m, e), c.push(_), g && !v && (v = _.hasChanged(y))
-                                        }
-                                        h[_.cid] || (h[_.cid] = !0, a.push(_)), t[s] = _
-                                    } else f && (o = t[s] = this._prepareModel(o, e)) && (u.push(o), this._addReference(o, e), h[o.cid] = !0, a.push(o))
+                    return o = {
+                        next: s(0),
+                        throw: s(1),
+                        return: s(2)
+                    }, "function" == typeof Symbol && (o[Symbol.iterator] = function() {
+                        return this
+                    }), o;
+
+                    function s(o) {
+                        return function(s) {
+                            return function(o) {
+                                if (r) throw new TypeError("Generator is already executing.");
+                                for (; u;) try {
+                                    if (r = 1, n && (i = 2 & o[0] ? n.return : o[0] ? n.throw || ((i = n.return) && i.call(n), 0) : n.next) && !(i = i.call(n, o[1])).done) return i;
+                                    switch (n = 0, i && (o = [2 & o[0], i.value]), o[0]) {
+                                        case 0:
+                                        case 1:
+                                            i = o;
+                                            break;
+                                        case 4:
+                                            return u.label++, {
+                                                value: o[1],
+                                                done: !1
+                                            };
+                                        case 5:
+                                            u.label++, n = o[1], o = [0];
+                                            continue;
+                                        case 7:
+                                            o = u.ops.pop(), u.trys.pop();
+                                            continue;
+                                        default:
+                                            if (!((i = (i = u.trys).length > 0 && i[i.length - 1]) || 6 !== o[0] && 2 !== o[0])) {
+                                                u = 0;
+                                                continue
+                                            }
+                                            if (3 === o[0] && (!i || o[1] > i[0] && o[1] < i[3])) {
+                                                u.label = o[1];
+                                                break
+                                            }
+                                            if (6 === o[0] && u.label < i[1]) {
+                                                u.label = i[1], i = o;
+                                                break
+                                            }
+                                            if (i && u.label < i[2]) {
+                                                u.label = i[2], u.ops.push(o);
+                                                break
+                                            }
+                                            i[2] && u.ops.pop(), u.trys.pop();
+                                            continue
+                                    }
+                                    o = e.call(t, u)
+                                } catch (t) {
+                                    o = [6, t], n = 0
+                                } finally {
+                                    r = i = 0
                                 }
-                                if (d) {
-                                    for (s = 0; s < this.length; s++) h[(o = this.models[s]).cid] || l.push(o);
-                                    l.length && this._removeModels(l, e)
-                                }
-                                var j = !1,
-                                    w = !g && f && d;
-                                if (a.length && w ? (j = this.length !== a.length || r.some(this.models, (function(t, e) {
-                                        return t !== a[e]
-                                    })), this.models.length = 0, x(this.models, a, 0), this.length = this.models.length) : u.length && (g && (v = !0), x(this.models, u, null == i ? this.length : i), this.length = this.models.length), v && this.sort({
-                                        silent: !0
-                                    }), !e.silent) {
-                                    for (s = 0; s < u.length; s++) null != i && (e.index = i + s), (o = u[s]).trigger("add", o, this, e);
-                                    (v || j) && this.trigger("sort", this, e), (u.length || l.length || c.length) && (e.changes = {
-                                        added: u,
-                                        removed: l,
-                                        merged: c
-                                    }, this.trigger("update", this, e))
+                                if (5 & o[0]) throw o[1];
+                                return {
+                                    value: o[0] ? o[1] : void 0,
+                                    done: !0
                                 }
-                                return n ? t[0] : t
-                            }
-                        },
-                        reset: function(t, e) {
-                            e = e ? r.clone(e) : {};
-                            for (var n = 0; n < this.models.length; n++) this._removeReference(this.models[n], e);
-                            return e.previousModels = this.models, this._reset(), t = this.add(t, r.extend({
-                                silent: !0
-                            }, e)), e.silent || this.trigger("reset", this, e), t
-                        },
-                        push: function(t, e) {
-                            return this.add(t, r.extend({
-                                at: this.length
-                            }, e))
-                        },
-                        pop: function(t) {
-                            var e = this.at(this.length - 1);
-                            return this.remove(e, t)
-                        },
-                        unshift: function(t, e) {
-                            return this.add(t, r.extend({
-                                at: 0
-                            }, e))
-                        },
-                        shift: function(t) {
-                            var e = this.at(0);
-                            return this.remove(e, t)
-                        },
-                        slice: function() {
-                            return o.apply(this.models, arguments)
-                        },
-                        get: function(t) {
-                            if (null != t) return this._byId[t] || this._byId[this.modelId(this._isModel(t) ? t.attributes : t)] || t.cid && this._byId[t.cid]
-                        },
-                        has: function(t) {
-                            return null != this.get(t)
-                        },
-                        at: function(t) {
-                            return t < 0 && (t += this.length), this.models[t]
-                        },
-                        where: function(t, e) {
-                            return this[e ? "find" : "filter"](t)
-                        },
-                        findWhere: function(t) {
-                            return this.where(t, !0)
-                        },
-                        sort: function(t) {
-                            var e = this.comparator;
-                            if (!e) throw new Error("Cannot sort a set without a comparator");
-                            t || (t = {});
-                            var n = e.length;
-                            return r.isFunction(e) && (e = e.bind(this)), 1 === n || r.isString(e) ? this.models = this.sortBy(e) : this.models.sort(e), t.silent || this.trigger("sort", this, t), this
-                        },
-                        pluck: function(t) {
-                            return this.map(t + "")
-                        },
-                        fetch: function(t) {
-                            var e = (t = r.extend({
-                                    parse: !0
-                                }, t)).success,
-                                n = this;
-                            return t.success = function(r) {
-                                var i = t.reset ? "reset" : "set";
-                                n[i](r, t), e && e.call(t.context, n, r, t), n.trigger("sync", n, r, t)
-                            }, q(this, t), this.sync("read", this, t)
-                        },
-                        create: function(t, e) {
-                            var n = (e = e ? r.clone(e) : {}).wait;
-                            if (!(t = this._prepareModel(t, e))) return !1;
-                            n || this.add(t, e);
-                            var i = this,
-                                o = e.success;
-                            return e.success = function(t, e, r) {
-                                n && i.add(t, r), o && o.call(r.context, t, e, r)
-                            }, t.save(null, e), t
-                        },
-                        parse: function(t, e) {
-                            return t
-                        },
-                        clone: function() {
-                            return new this.constructor(this.models, {
-                                model: this.model,
-                                comparator: this.comparator
-                            })
-                        },
-                        modelId: function(t) {
-                            return t[this.model.prototype.idAttribute || "id"]
-                        },
-                        values: function() {
-                            return new w(this, O)
-                        },
-                        keys: function() {
-                            return new w(this, S)
-                        },
-                        entries: function() {
-                            return new w(this, E)
-                        },
-                        _reset: function() {
-                            this.length = 0, this.models = [], this._byId = {}
-                        },
-                        _prepareModel: function(t, e) {
-                            if (this._isModel(t)) return t.collection || (t.collection = this), t;
-                            (e = e ? r.clone(e) : {}).collection = this;
-                            var n = new this.model(t, e);
-                            return n.validationError ? (this.trigger("invalid", this, n.validationError, e), !1) : n
-                        },
-                        _removeModels: function(t, e) {
-                            for (var r = [], n = 0; n < t.length; n++) {
-                                var i = this.get(t[n]);
-                                if (i) {
-                                    var o = this.indexOf(i);
-                                    this.models.splice(o, 1), this.length--, delete this._byId[i.cid];
-                                    var s = this.modelId(i.attributes);
-                                    null != s && delete this._byId[s], e.silent || (e.index = o, i.trigger("remove", i, this, e)), r.push(i), this._removeReference(i, e)
+                            }([o, s])
+                        }
+                    }
+                };
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.HubControl = void 0;
+            var u = r(545),
+                s = r(467),
+                c = function() {
+                    function t(t, e, r) {
+                        this.hub = null, this.device = t, this.control = e, this.configuration = r, this.prevControl = n({}, this.control), this.states = {
+                            Turn: s.turn,
+                            Drive: s.drive,
+                            Stop: s.stop,
+                            Back: s.back,
+                            Manual: u.manual,
+                            Seek: s.seek
+                        }, this.currentState = this.states.Manual
+                    }
+                    return t.prototype.updateConfiguration = function(t) {
+                        this.configuration = t
+                    }, t.prototype.start = function(t) {
+                        return i(this, void 0, void 0, (function() {
+                            var e = this;
+                            return o(this, (function(r) {
+                                switch (r.label) {
+                                    case 0:
+                                        return this.hub = t, this.device.connected = !0, this.hub.emitter.on("error", (function(t) {
+                                            e.device.err = t
+                                        })), this.hub.emitter.on("disconnect", (function() {
+                                            e.device.connected = !1
+                                        })), this.hub.emitter.on("distance", (function(t) {
+                                            e.device.distance = t
+                                        })), this.hub.emitter.on("rssi", (function(t) {
+                                            e.device.rssi = t
+                                        })), this.hub.emitter.on("port", (function(t) {
+                                            var r = t.port,
+                                                n = t.action;
+                                            e.device.ports[r].action = n
+                                        })), this.hub.emitter.on("color", (function(t) {
+                                            e.device.color = t
+                                        })), this.hub.emitter.on("tilt", (function(t) {
+                                            var r = t.roll,
+                                                n = t.pitch;
+                                            e.device.tilt.roll = r, e.device.tilt.pitch = n
+                                        })), this.hub.emitter.on("rotation", (function(t) {
+                                            var r = t.port,
+                                                n = t.angle;
+                                            e.device.ports[r].angle = n
+                                        })), [4, this.hub.ledAsync("red")];
+                                    case 1:
+                                        return r.sent(), [4, this.hub.ledAsync("yellow")];
+                                    case 2:
+                                        return r.sent(), [4, this.hub.ledAsync("green")];
+                                    case 3:
+                                        return r.sent(), [2]
                                 }
-                            }
-                            return r
-                        },
-                        _isModel: function(t) {
-                            return t instanceof y
-                        },
-                        _addReference: function(t, e) {
-                            this._byId[t.cid] = t;
-                            var r = this.modelId(t.attributes);
-                            null != r && (this._byId[r] = t), t.on("all", this._onModelEvent, this)
-                        },
-                        _removeReference: function(t, e) {
-                            delete this._byId[t.cid];
-                            var r = this.modelId(t.attributes);
-                            null != r && delete this._byId[r], this === t.collection && delete t.collection, t.off("all", this._onModelEvent, this)
-                        },
-                        _onModelEvent: function(t, e, r, n) {
-                            if (e) {
-                                if (("add" === t || "remove" === t) && r !== this) return;
-                                if ("destroy" === t && this.remove(e, n), "change" === t) {
-                                    var i = this.modelId(e.previousAttributes()),
-                                        o = this.modelId(e.attributes);
-                                    i !== o && (null != i && delete this._byId[i], null != o && (this._byId[o] = e))
+                            }))
+                        }))
+                    }, t.prototype.disconnect = function() {
+                        return i(this, void 0, void 0, (function() {
+                            return o(this, (function(t) {
+                                switch (t.label) {
+                                    case 0:
+                                        return this.device.connected ? [4, this.hub.disconnectAsync()] : [3, 2];
+                                    case 1:
+                                        t.sent(), t.label = 2;
+                                    case 2:
+                                        return [2]
                                 }
+                            }))
+                        }))
+                    }, t.prototype.setNextState = function(t) {
+                        this.control.controlUpdateTime = void 0, this.control.state = t, this.currentState = this.states[t]
+                    }, t.prototype.update = function() {
+                        this.currentState(this), this.prevControl = n({}, this.control), this.prevControl.tilt = n({}, this.control.tilt), this.prevDevice = n({}, this.device)
+                    }, t
+                }();
+            e.HubControl = c
+        },
+        467: (t, e) => {
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.seek = e.turn = e.drive = e.back = e.stop = void 0;
+            var r = 59e3;
+            e.seek = function(t) {
+                (!t.control.controlUpdateTime || Date.now() - t.control.controlUpdateTime > r) && (t.control.controlUpdateTime = Date.now(), t.hub.motorTimeMulti(60, 30, -10)), Date.now() - t.control.controlUpdateTime < 250 || (t.device.distance > t.prevDevice.distance ? (t.control.turnDirection = "right", t.setNextState("Turn")) : (t.control.turnDirection = "left", t.setNextState("Turn")))
+            }, e.turn = function(t) {
+                if (t.device.distance < 75) return t.control.turnDirection = null, void t.setNextState("Back");
+                if (t.device.distance > 100) return t.control.turnDirection = null, void t.setNextState("Drive");
+                if (!t.control.controlUpdateTime || Date.now() - t.control.controlUpdateTime > r) {
+                    var e = "right" === t.control.turnDirection ? 30 : -10,
+                        n = "right" === t.control.turnDirection ? -10 : 30;
+                    t.control.controlUpdateTime = Date.now(), t.hub.motorTimeMulti(60, e, n)
+                }
+            }, e.drive = function(t) {
+                if (t.device.distance < 75) t.setNextState("Back");
+                else if (t.device.distance < 100) t.setNextState("Seek");
+                else if (!t.control.controlUpdateTime || Date.now() - t.control.controlUpdateTime > r) {
+                    t.control.controlUpdateTime = Date.now();
+                    var e = "A" === t.configuration.leftMotor ? 30 : -30;
+                    t.hub.motorTimeMulti(60, e, e)
+                }
+            }, e.back = function(t) {
+                if (t.device.distance > 100) t.setNextState("Seek");
+                else if (!t.control.controlUpdateTime || Date.now() - t.control.controlUpdateTime > r) {
+                    t.control.controlUpdateTime = Date.now();
+                    var e = "A" === t.configuration.leftMotor ? -15 : 15;
+                    t.hub.motorTimeMulti(60, e, e)
+                }
+            }, e.stop = function(t) {
+                t.control.speed = 0, t.control.turnAngle = 0, (!t.control.controlUpdateTime || Date.now() - t.control.controlUpdateTime > r) && (t.control.controlUpdateTime = Date.now(), t.hub.motorTimeMulti(60, 0, 0))
+            }
+        },
+        545: (t, e) => {
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.manual = void 0, e.manual = function(t) {
+                if (t.control.speed !== t.prevControl.speed || t.control.turnAngle !== t.prevControl.turnAngle) {
+                    var e = t.control.speed + (t.control.turnAngle > 0 ? Math.abs(t.control.turnAngle) : 0),
+                        r = t.control.speed + (t.control.turnAngle < 0 ? Math.abs(t.control.turnAngle) : 0);
+                    e > 100 && (r -= e - 100, e = 100), r > 100 && (e -= r - 100, r = 100), t.control.motorA = e, t.control.motorB = r, t.hub.motorTimeMulti(60, e, r)
+                }
+                t.control.tilt.pitch !== t.prevControl.tilt.pitch && t.hub.motorTime("C", 60, t.control.tilt.pitch), t.control.tilt.roll !== t.prevControl.tilt.roll && t.hub.motorTime("D", 60, t.control.tilt.roll)
+            }
+        },
+        990: function(t, e) {
+            var r = this && this.__awaiter || function(t, e, r, n) {
+                    return new(r || (r = Promise))((function(i, o) {
+                        function u(t) {
+                            try {
+                                c(n.next(t))
+                            } catch (t) {
+                                o(t)
                             }
-                            this.trigger.apply(this, arguments)
                         }
-                    });
-                    var j = "function" == typeof Symbol && Symbol.iterator;
-                    j && (_.prototype[j] = _.prototype.values);
-                    var w = function(t, e) {
-                            this._collection = t, this._kind = e, this._index = 0
-                        },
-                        O = 1,
-                        S = 2,
-                        E = 3;
-                    j && (w.prototype[j] = function() {
-                        return this
-                    }), w.prototype.next = function() {
-                        if (this._collection) {
-                            if (this._index < this._collection.length) {
-                                var t, e = this._collection.at(this._index);
-                                if (this._index++, this._kind === O) t = e;
-                                else {
-                                    var r = this._collection.modelId(e.attributes);
-                                    t = this._kind === S ? r : [r, e]
-                                }
-                                return {
-                                    value: t,
-                                    done: !1
-                                }
+
+                        function s(t) {
+                            try {
+                                c(n.throw(t))
+                            } catch (t) {
+                                o(t)
                             }
-                            this._collection = void 0
                         }
-                        return {
-                            value: void 0,
-                            done: !0
+
+                        function c(t) {
+                            var e;
+                            t.done ? i(t.value) : (e = t.value, e instanceof r ? e : new r((function(t) {
+                                t(e)
+                            }))).then(u, s)
                         }
-                    };
-                    var A = e.View = function(t) {
-                            this.cid = r.uniqueId("view"), this.preinitialize.apply(this, arguments), r.extend(this, r.pick(t, I)), this._ensureElement(), this.initialize.apply(this, arguments)
-                        },
-                        k = /^(\S+)\s*(.*)$/,
-                        I = ["model", "collection", "el", "id", "attributes", "className", "tagName", "events"];
-                    r.extend(A.prototype, a, {
-                        tagName: "div",
-                        $: function(t) {
-                            return this.$el.find(t)
-                        },
-                        preinitialize: function() {},
-                        initialize: function() {},
-                        render: function() {
-                            return this
-                        },
-                        remove: function() {
-                            return this._removeElement(), this.stopListening(), this
-                        },
-                        _removeElement: function() {
-                            this.$el.remove()
-                        },
-                        setElement: function(t) {
-                            return this.undelegateEvents(), this._setElement(t), this.delegateEvents(), this
-                        },
-                        _setElement: function(t) {
-                            this.$el = t instanceof e.$ ? t : e.$(t), this.el = this.$el[0]
-                        },
-                        delegateEvents: function(t) {
-                            if (t || (t = r.result(this, "events")), !t) return this;
-                            for (var e in this.undelegateEvents(), t) {
-                                var n = t[e];
-                                if (r.isFunction(n) || (n = this[n]), n) {
-                                    var i = e.match(k);
-                                    this.delegate(i[1], i[2], n.bind(this))
-                                }
-                            }
-                            return this
-                        },
-                        delegate: function(t, e, r) {
-                            return this.$el.on(t + ".delegateEvents" + this.cid, e, r), this
-                        },
-                        undelegateEvents: function() {
-                            return this.$el && this.$el.off(".delegateEvents" + this.cid), this
-                        },
-                        undelegate: function(t, e, r) {
-                            return this.$el.off(t + ".delegateEvents" + this.cid, e, r), this
-                        },
-                        _createElement: function(t) {
-                            return document.createElement(t)
-                        },
-                        _ensureElement: function() {
-                            if (this.el) this.setElement(r.result(this, "el"));
-                            else {
-                                var t = r.extend({}, r.result(this, "attributes"));
-                                this.id && (t.id = r.result(this, "id")), this.className && (t.class = r.result(this, "className")), this.setElement(this._createElement(r.result(this, "tagName"))), this._setAttributes(t)
-                            }
+                        c((n = n.apply(t, e || [])).next())
+                    }))
+                },
+                n = this && this.__generator || function(t, e) {
+                    var r, n, i, o, u = {
+                        label: 0,
+                        sent: function() {
+                            if (1 & i[0]) throw i[1];
+                            return i[1]
                         },
-                        _setAttributes: function(t) {
-                            this.$el.attr(t)
-                        }
-                    });
-                    var T = function(t, e, n, i) {
-                            r.each(n, (function(r, n) {
-                                e[n] && (t.prototype[n] = function(t, e, r, n) {
-                                    switch (e) {
+                        trys: [],
+                        ops: []
+                    };
+                    return o = {
+                        next: s(0),
+                        throw: s(1),
+                        return: s(2)
+                    }, "function" == typeof Symbol && (o[Symbol.iterator] = function() {
+                        return this
+                    }), o;
+
+                    function s(o) {
+                        return function(s) {
+                            return function(o) {
+                                if (r) throw new TypeError("Generator is already executing.");
+                                for (; u;) try {
+                                    if (r = 1, n && (i = 2 & o[0] ? n.return : o[0] ? n.throw || ((i = n.return) && i.call(n), 0) : n.next) && !(i = i.call(n, o[1])).done) return i;
+                                    switch (n = 0, i && (o = [2 & o[0], i.value]), o[0]) {
+                                        case 0:
                                         case 1:
-                                            return function() {
-                                                return t[r](this[n])
-                                            };
-                                        case 2:
-                                            return function(e) {
-                                                return t[r](this[n], e)
-                                            };
-                                        case 3:
-                                            return function(e, i) {
-                                                return t[r](this[n], P(e, this), i)
-                                            };
+                                            i = o;
+                                            break;
                                         case 4:
-                                            return function(e, i, o) {
-                                                return t[r](this[n], P(e, this), i, o)
+                                            return u.label++, {
+                                                value: o[1],
+                                                done: !1
                                             };
+                                        case 5:
+                                            u.label++, n = o[1], o = [0];
+                                            continue;
+                                        case 7:
+                                            o = u.ops.pop(), u.trys.pop();
+                                            continue;
                                         default:
-                                            return function() {
-                                                var e = o.call(arguments);
-                                                return e.unshift(this[n]), t[r].apply(t, e)
+                                            if (!((i = (i = u.trys).length > 0 && i[i.length - 1]) || 6 !== o[0] && 2 !== o[0])) {
+                                                u = 0;
+                                                continue
+                                            }
+                                            if (3 === o[0] && (!i || o[1] > i[0] && o[1] < i[3])) {
+                                                u.label = o[1];
+                                                break
+                                            }
+                                            if (6 === o[0] && u.label < i[1]) {
+                                                u.label = i[1], i = o;
+                                                break
                                             }
+                                            if (i && u.label < i[2]) {
+                                                u.label = i[2], u.ops.push(o);
+                                                break
+                                            }
+                                            i[2] && u.ops.pop(), u.trys.pop();
+                                            continue
                                     }
-                                }(e, r, n, i))
-                            }))
-                        },
-                        P = function(t, e) {
-                            return r.isFunction(t) ? t : r.isObject(t) && !e._isModel(t) ? M(t) : r.isString(t) ? function(e) {
-                                return e.get(t)
-                            } : t
-                        },
-                        M = function(t) {
-                            var e = r.matches(t);
-                            return function(t) {
-                                return e(t.attributes)
-                            }
-                        };
-                    r.each([
-                        [_, {
-                            forEach: 3,
-                            each: 3,
-                            map: 3,
-                            collect: 3,
-                            reduce: 0,
-                            foldl: 0,
-                            inject: 0,
-                            reduceRight: 0,
-                            foldr: 0,
-                            find: 3,
-                            detect: 3,
-                            filter: 3,
-                            select: 3,
-                            reject: 3,
-                            every: 3,
-                            all: 3,
-                            some: 3,
-                            any: 3,
-                            include: 3,
-                            includes: 3,
-                            contains: 3,
-                            invoke: 0,
-                            max: 3,
-                            min: 3,
-                            toArray: 1,
-                            size: 1,
-                            first: 3,
-                            head: 3,
-                            take: 3,
-                            initial: 3,
-                            rest: 3,
-                            tail: 3,
-                            drop: 3,
-                            last: 3,
-                            without: 0,
-                            difference: 0,
-                            indexOf: 3,
-                            shuffle: 1,
-                            lastIndexOf: 3,
-                            isEmpty: 1,
-                            chain: 1,
-                            sample: 3,
-                            partition: 3,
-                            groupBy: 3,
-                            countBy: 3,
-                            sortBy: 3,
-                            indexBy: 3,
-                            findIndex: 3,
-                            findLastIndex: 3
-                        }, "models"],
-                        [y, {
-                            keys: 1,
-                            values: 1,
-                            pairs: 1,
-                            invert: 1,
-                            pick: 0,
-                            omit: 0,
-                            chain: 1,
-                            isEmpty: 1
-                        }, "attributes"]
-                    ], (function(t) {
-                        var e = t[0],
-                            n = t[1],
-                            i = t[2];
-                        e.mixin = function(t) {
-                            var n = r.reduce(r.functions(t), (function(t, e) {
-                                return t[e] = 0, t
-                            }), {});
-                            T(e, t, n, i)
-                        }, T(e, r, n, i)
-                    })), e.sync = function(t, n, i) {
-                        var o = z[t];
-                        r.defaults(i || (i = {}), {
-                            emulateHTTP: e.emulateHTTP,
-                            emulateJSON: e.emulateJSON
-                        });
-                        var s = {
-                            type: o,
-                            dataType: "json"
-                        };
-                        if (i.url || (s.url = r.result(n, "url") || L()), null != i.data || !n || "create" !== t && "update" !== t && "patch" !== t || (s.contentType = "application/json", s.data = JSON.stringify(i.attrs || n.toJSON(i))), i.emulateJSON && (s.contentType = "application/x-www-form-urlencoded", s.data = s.data ? {
-                                model: s.data
-                            } : {}), i.emulateHTTP && ("PUT" === o || "DELETE" === o || "PATCH" === o)) {
-                            s.type = "POST", i.emulateJSON && (s.data._method = o);
-                            var a = i.beforeSend;
-                            i.beforeSend = function(t) {
-                                if (t.setRequestHeader("X-HTTP-Method-Override", o), a) return a.apply(this, arguments)
-                            }
+                                    o = e.call(t, u)
+                                } catch (t) {
+                                    o = [6, t], n = 0
+                                } finally {
+                                    r = i = 0
+                                }
+                                if (5 & o[0]) throw o[1];
+                                return {
+                                    value: o[0] ? o[1] : void 0,
+                                    done: !0
+                                }
+                            }([o, s])
                         }
-                        "GET" === s.type || i.emulateJSON || (s.processData = !1);
-                        var u = i.error;
-                        i.error = function(t, e, r) {
-                            i.textStatus = e, i.errorThrown = r, u && u.call(i.context, t, e, r)
-                        };
-                        var c = i.xhr = e.ajax(r.extend(s, i));
-                        return n.trigger("request", n, c, i), c
-                    };
-                    var z = {
-                        create: "POST",
-                        update: "PUT",
-                        patch: "PATCH",
-                        delete: "DELETE",
-                        read: "GET"
-                    };
-                    e.ajax = function() {
-                        return e.$.ajax.apply(e.$, arguments)
-                    };
-                    var N = e.Router = function(t) {
-                            t || (t = {}), this.preinitialize.apply(this, arguments), t.routes && (this.routes = t.routes), this._bindRoutes(), this.initialize.apply(this, arguments)
-                        },
-                        $ = /\((.*?)\)/g,
-                        R = /(\(\?)?:\w+/g,
-                        B = /\*\w+/g,
-                        C = /[\-{}\[\]+?.,\\\^$|#\s]/g;
-                    r.extend(N.prototype, a, {
-                        preinitialize: function() {},
-                        initialize: function() {},
-                        route: function(t, n, i) {
-                            r.isRegExp(t) || (t = this._routeToRegExp(t)), r.isFunction(n) && (i = n, n = ""), i || (i = this[n]);
-                            var o = this;
-                            return e.history.route(t, (function(r) {
-                                var s = o._extractParameters(t, r);
-                                !1 !== o.execute(i, s, n) && (o.trigger.apply(o, ["route:" + n].concat(s)), o.trigger("route", n, s), e.history.trigger("route", o, n, s))
-                            })), this
-                        },
-                        execute: function(t, e, r) {
-                            t && t.apply(this, e)
-                        },
-                        navigate: function(t, r) {
-                            return e.history.navigate(t, r), this
-                        },
-                        _bindRoutes: function() {
-                            if (this.routes) {
-                                this.routes = r.result(this, "routes");
-                                for (var t, e = r.keys(this.routes); null != (t = e.pop());) this.route(t, this.routes[t])
-                            }
-                        },
-                        _routeToRegExp: function(t) {
-                            return t = t.replace(C, "\\$&").replace($, "(?:$1)?").replace(R, (function(t, e) {
-                                return e ? t : "([^/?]+)"
-                            })).replace(B, "([^?]*?)"), new RegExp("^" + t + "(?:\\?([\\s\\S]*))?$")
-                        },
-                        _extractParameters: function(t, e) {
-                            var n = t.exec(e).slice(1);
-                            return r.map(n, (function(t, e) {
-                                return e === n.length - 1 ? t || null : t ? decodeURIComponent(t) : null
+                    }
+                };
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.BoostConnector = void 0;
+            var i = "00001623-1212-efde-1623-785feabcd123",
+                o = function() {
+                    function t() {}
+                    return t.connect = function(e) {
+                        return r(this, void 0, void 0, (function() {
+                            var o, u, s = this;
+                            return n(this, (function(c) {
+                                switch (c.label) {
+                                    case 0:
+                                        return o = {
+                                            acceptAllDevices: !1,
+                                            filters: [{
+                                                services: [i]
+                                            }],
+                                            optionalServices: [i]
+                                        }, u = this, [4, navigator.bluetooth.requestDevice(o)];
+                                    case 1:
+                                        return u.device = c.sent(), this.device.addEventListener("gattserverdisconnected", (function(t) {
+                                            return r(s, void 0, void 0, (function() {
+                                                return n(this, (function(t) {
+                                                    switch (t.label) {
+                                                        case 0:
+                                                            return [4, e()];
+                                                        case 1:
+                                                            return t.sent(), [2]
+                                                    }
+                                                }))
+                                            }))
+                                        })), [2, t.getCharacteristic(this.device)]
+                                }
                             }))
-                        }
-                    });
-                    var U = e.History = function() {
-                            this.handlers = [], this.checkUrl = this.checkUrl.bind(this), "undefined" != typeof window && (this.location = window.location, this.history = window.history)
-                        },
-                        F = /^[#\/]|\s+$/g,
-                        H = /^\/+|\/+$/g,
-                        D = /#.*$/;
-                    U.started = !1, r.extend(U.prototype, a, {
-                        interval: 50,
-                        atRoot: function() {
-                            return this.location.pathname.replace(/[^\/]$/, "$&/") === this.root && !this.getSearch()
-                        },
-                        matchRoot: function() {
-                            return this.decodeFragment(this.location.pathname).slice(0, this.root.length - 1) + "/" === this.root
-                        },
-                        decodeFragment: function(t) {
-                            return decodeURI(t.replace(/%25/g, "%2525"))
-                        },
-                        getSearch: function() {
-                            var t = this.location.href.replace(/#.*/, "").match(/\?.+/);
-                            return t ? t[0] : ""
-                        },
-                        getHash: function(t) {
-                            var e = (t || this).location.href.match(/#(.*)$/);
-                            return e ? e[1] : ""
-                        },
-                        getPath: function() {
-                            var t = this.decodeFragment(this.location.pathname + this.getSearch()).slice(this.root.length - 1);
-                            return "/" === t.charAt(0) ? t.slice(1) : t
-                        },
-                        getFragment: function(t) {
-                            return null == t && (t = this._usePushState || !this._wantsHashChange ? this.getPath() : this.getHash()), t.replace(F, "")
-                        },
-                        start: function(t) {
-                            if (U.started) throw new Error("Backbone.history has already been started");
-                            if (U.started = !0, this.options = r.extend({
-                                    root: "/"
-                                }, this.options, t), this.root = this.options.root, this._wantsHashChange = !1 !== this.options.hashChange, this._hasHashChange = "onhashchange" in window && (void 0 === document.documentMode || document.documentMode > 7), this._useHashChange = this._wantsHashChange && this._hasHashChange, this._wantsPushState = !!this.options.pushState, this._hasPushState = !(!this.history || !this.history.pushState), this._usePushState = this._wantsPushState && this._hasPushState, this.fragment = this.getFragment(), this.root = ("/" + this.root + "/").replace(H, "/"), this._wantsHashChange && this._wantsPushState) {
-                                if (!this._hasPushState && !this.atRoot()) {
-                                    var e = this.root.slice(0, -1) || "/";
-                                    return this.location.replace(e + "#" + this.getPath()), !0
-                                }
-                                this._hasPushState && this.atRoot() && this.navigate(this.getHash(), {
-                                    replace: !0
-                                })
-                            }
-                            if (!this._hasHashChange && this._wantsHashChange && !this._usePushState) {
-                                this.iframe = document.createElement("iframe"), this.iframe.src = "javascript:0", this.iframe.style.display = "none", this.iframe.tabIndex = -1;
-                                var n = document.body,
-                                    i = n.insertBefore(this.iframe, n.firstChild).contentWindow;
-                                i.document.open(), i.document.close(), i.location.hash = "#" + this.fragment
-                            }
-                            var o = window.addEventListener || function(t, e) {
-                                return attachEvent("on" + t, e)
-                            };
-                            if (this._usePushState ? o("popstate", this.checkUrl, !1) : this._useHashChange && !this.iframe ? o("hashchange", this.checkUrl, !1) : this._wantsHashChange && (this._checkUrlInterval = setInterval(this.checkUrl, this.interval)), !this.options.silent) return this.loadUrl()
-                        },
-                        stop: function() {
-                            var t = window.removeEventListener || function(t, e) {
-                                return detachEvent("on" + t, e)
-                            };
-                            this._usePushState ? t("popstate", this.checkUrl, !1) : this._useHashChange && !this.iframe && t("hashchange", this.checkUrl, !1), this.iframe && (document.body.removeChild(this.iframe), this.iframe = null), this._checkUrlInterval && clearInterval(this._checkUrlInterval), U.started = !1
-                        },
-                        route: function(t, e) {
-                            this.handlers.unshift({
-                                route: t,
-                                callback: e
-                            })
-                        },
-                        checkUrl: function(t) {
-                            var e = this.getFragment();
-                            if (e === this.fragment && this.iframe && (e = this.getHash(this.iframe.contentWindow)), e === this.fragment) return !1;
-                            this.iframe && this.navigate(e), this.loadUrl()
-                        },
-                        loadUrl: function(t) {
-                            return !!this.matchRoot() && (t = this.fragment = this.getFragment(t), r.some(this.handlers, (function(e) {
-                                if (e.route.test(t)) return e.callback(t), !0
-                            })))
-                        },
-                        navigate: function(t, e) {
-                            if (!U.started) return !1;
-                            e && !0 !== e || (e = {
-                                trigger: !!e
-                            }), t = this.getFragment(t || "");
-                            var r = this.root;
-                            "" !== t && "?" !== t.charAt(0) || (r = r.slice(0, -1) || "/");
-                            var n = r + t;
-                            t = t.replace(D, "");
-                            var i = this.decodeFragment(t);
-                            if (this.fragment !== i) {
-                                if (this.fragment = i, this._usePushState) this.history[e.replace ? "replaceState" : "pushState"]({}, document.title, n);
-                                else {
-                                    if (!this._wantsHashChange) return this.location.assign(n);
-                                    if (this._updateHash(this.location, t, e.replace), this.iframe && t !== this.getHash(this.iframe.contentWindow)) {
-                                        var o = this.iframe.contentWindow;
-                                        e.replace || (o.document.open(), o.document.close()), this._updateHash(o.location, t, e.replace)
-                                    }
+                        }))
+                    }, t.getCharacteristic = function(t) {
+                        return r(this, void 0, void 0, (function() {
+                            return n(this, (function(e) {
+                                switch (e.label) {
+                                    case 0:
+                                        return [4, t.gatt.connect()];
+                                    case 1:
+                                        return [4, e.sent().getPrimaryService(i)];
+                                    case 2:
+                                        return [4, e.sent().getCharacteristic("00001624-1212-efde-1623-785feabcd123")];
+                                    case 3:
+                                        return [2, e.sent()]
                                 }
-                                return e.trigger ? this.loadUrl(t) : void 0
-                            }
-                        },
-                        _updateHash: function(t, e, r) {
-                            if (r) {
-                                var n = t.href.replace(/(javascript:|#).*$/, "");
-                                t.replace(n + "#" + e)
-                            } else t.hash = "#" + e
-                        }
-                    }), e.history = new U;
-                    y.extend = _.extend = N.extend = A.extend = U.extend = function(t, e) {
-                        var n, i = this;
-                        return n = t && r.has(t, "constructor") ? t.constructor : function() {
-                            return i.apply(this, arguments)
-                        }, r.extend(n, i, e), n.prototype = r.create(i.prototype, t), n.prototype.constructor = n, n.__super__ = i.prototype, n
-                    };
-                    var L = function() {
-                            throw new Error('A "url" property or function must be specified')
-                        },
-                        q = function(t, e) {
-                            var r = e.error;
-                            e.error = function(n) {
-                                r && r.call(e.context, t, n, e), t.trigger("error", t, n, e)
-                            }
-                        };
-                    return e
-                }(o, r, t, e)
-            }.apply(e, n), void 0 === i || (t.exports = i)
-        },
-        9515: (t, e, r) => {
-            var n = r(8761)(r(7772), "DataView");
-            t.exports = n
-        },
-        9612: (t, e, r) => {
-            var n = r(2118),
-                i = r(6909),
-                o = r(8138),
-                s = r(4174),
-                a = r(7942);
-
-            function u(t) {
-                var e = -1,
-                    r = null == t ? 0 : t.length;
-                for (this.clear(); ++e < r;) {
-                    var n = t[e];
-                    this.set(n[0], n[1])
-                }
-            }
-            u.prototype.clear = n, u.prototype.delete = i, u.prototype.get = o, u.prototype.has = s, u.prototype.set = a, t.exports = u
-        },
-        235: (t, e, r) => {
-            var n = r(3945),
-                i = r(1846),
-                o = r(8028),
-                s = r(2344),
-                a = r(4769);
-
-            function u(t) {
-                var e = -1,
-                    r = null == t ? 0 : t.length;
-                for (this.clear(); ++e < r;) {
-                    var n = t[e];
-                    this.set(n[0], n[1])
-                }
-            }
-            u.prototype.clear = n, u.prototype.delete = i, u.prototype.get = o, u.prototype.has = s, u.prototype.set = a, t.exports = u
-        },
-        326: (t, e, r) => {
-            var n = r(8761)(r(7772), "Map");
-            t.exports = n
-        },
-        6738: (t, e, r) => {
-            var n = r(2411),
-                i = r(6417),
-                o = r(6928),
-                s = r(9493),
-                a = r(4150);
-
-            function u(t) {
-                var e = -1,
-                    r = null == t ? 0 : t.length;
-                for (this.clear(); ++e < r;) {
-                    var n = t[e];
-                    this.set(n[0], n[1])
-                }
-            }
-            u.prototype.clear = n, u.prototype.delete = i, u.prototype.get = o, u.prototype.has = s, u.prototype.set = a, t.exports = u
-        },
-        2760: (t, e, r) => {
-            var n = r(8761)(r(7772), "Promise");
-            t.exports = n
-        },
-        2143: (t, e, r) => {
-            var n = r(8761)(r(7772), "Set");
-            t.exports = n
+                            }))
+                        }))
+                    }, t.reconnect = function() {
+                        return r(this, void 0, void 0, (function() {
+                            return n(this, (function(e) {
+                                switch (e.label) {
+                                    case 0:
+                                        return this.device ? [4, t.getCharacteristic(this.device)] : [3, 2];
+                                    case 1:
+                                        return [2, [!0, e.sent()]];
+                                    case 2:
+                                        return [2, [!1, null]]
+                                }
+                            }))
+                        }))
+                    }, t.disconnect = function() {
+                        return !!this.device && (this.device.gatt.disconnect(), !0)
+                    }, t.isWebBluetoothSupported = !!navigator.bluetooth, t
+                }();
+            e.BoostConnector = o
         },
-        5386: (t, e, r) => {
-            var n = r(6738),
-                i = r(2842),
-                o = r(2482);
+        67: (t, e, r) => {
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.kMaxLength = e.INSPECT_MAX_BYTES = e.SlowBuffer = e.Buffer = void 0;
+            var n = Promise.resolve().then((function() {
+                    return r(742)
+                })),
+                i = Promise.resolve().then((function() {
+                    return r(264)
+                }));
+            e.INSPECT_MAX_BYTES = 50;
+            var o = 2147483647,
+                u = o;
 
             function s(t) {
-                var e = -1,
-                    r = null == t ? 0 : t.length;
-                for (this.__data__ = new n; ++e < r;) this.add(t[e])
-            }
-            s.prototype.add = s.prototype.push = i, s.prototype.has = o, t.exports = s
-        },
-        6571: (t, e, r) => {
-            var n = r(235),
-                i = r(5243),
-                o = r(2858),
-                s = r(4417),
-                a = r(8605),
-                u = r(1418);
-
-            function c(t) {
-                var e = this.__data__ = new n(t);
-                this.size = e.size
-            }
-            c.prototype.clear = i, c.prototype.delete = o, c.prototype.get = s, c.prototype.has = a, c.prototype.set = u, t.exports = c
-        },
-        857: (t, e, r) => {
-            var n = r(7772).Symbol;
-            t.exports = n
-        },
-        9162: (t, e, r) => {
-            var n = r(7772).Uint8Array;
-            t.exports = n
-        },
-        3215: (t, e, r) => {
-            var n = r(8761)(r(7772), "WeakMap");
-            t.exports = n
-        },
-        7552: t => {
-            t.exports = function(t, e) {
-                for (var r = -1, n = null == t ? 0 : t.length, i = 0, o = []; ++r < n;) {
-                    var s = t[r];
-                    e(s, r, t) && (o[i++] = s)
-                }
-                return o
-            }
-        },
-        1634: (t, e, r) => {
-            var n = r(6473),
-                i = r(9631),
-                o = r(6152),
-                s = r(3226),
-                a = r(9045),
-                u = r(7598),
-                c = Object.prototype.hasOwnProperty;
-            t.exports = function(t, e) {
-                var r = o(t),
-                    l = !r && i(t),
-                    h = !r && !l && s(t),
-                    f = !r && !l && !h && u(t),
-                    p = r || l || h || f,
-                    d = p ? n(t.length, String) : [],
-                    v = d.length;
-                for (var g in t) !e && !c.call(t, g) || p && ("length" == g || h && ("offset" == g || "parent" == g) || f && ("buffer" == g || "byteLength" == g || "byteOffset" == g) || a(g, v)) || d.push(g);
-                return d
-            }
-        },
-        5067: t => {
-            t.exports = function(t, e) {
-                for (var r = -1, n = e.length, i = t.length; ++r < n;) t[i + r] = e[r];
-                return t
-            }
-        },
-        7064: t => {
-            t.exports = function(t, e) {
-                for (var r = -1, n = null == t ? 0 : t.length; ++r < n;)
-                    if (e(t[r], r, t)) return !0;
-                return !1
-            }
-        },
-        2218: (t, e, r) => {
-            var n = r(1225);
-            t.exports = function(t, e) {
-                for (var r = t.length; r--;)
-                    if (n(t[r][0], e)) return r;
-                return -1
-            }
-        },
-        1897: (t, e, r) => {
-            var n = r(5067),
-                i = r(6152);
-            t.exports = function(t, e, r) {
-                var o = e(t);
-                return i(t) ? o : n(o, r(t))
-            }
-        },
-        3366: (t, e, r) => {
-            var n = r(857),
-                i = r(2107),
-                o = r(7157),
-                s = n ? n.toStringTag : void 0;
-            t.exports = function(t) {
-                return null == t ? void 0 === t ? "[object Undefined]" : "[object Null]" : s && s in Object(t) ? i(t) : o(t)
-            }
-        },
-        5183: (t, e, r) => {
-            var n = r(3366),
-                i = r(5125);
-            t.exports = function(t) {
-                return i(t) && "[object Arguments]" == n(t)
-            }
-        },
-        8746: (t, e, r) => {
-            var n = r(1952),
-                i = r(5125);
-            t.exports = function t(e, r, o, s, a) {
-                return e === r || (null == e || null == r || !i(e) && !i(r) ? e != e && r != r : n(e, r, o, s, t, a))
-            }
-        },
-        1952: (t, e, r) => {
-            var n = r(6571),
-                i = r(4871),
-                o = r(1491),
-                s = r(7416),
-                a = r(940),
-                u = r(6152),
-                c = r(3226),
-                l = r(7598),
-                h = "[object Arguments]",
-                f = "[object Array]",
-                p = "[object Object]",
-                d = Object.prototype.hasOwnProperty;
-            t.exports = function(t, e, r, v, g, y) {
-                var _ = u(t),
-                    b = u(e),
-                    m = _ ? f : a(t),
-                    x = b ? f : a(e),
-                    j = (m = m == h ? p : m) == p,
-                    w = (x = x == h ? p : x) == p,
-                    O = m == x;
-                if (O && c(t)) {
-                    if (!c(e)) return !1;
-                    _ = !0, j = !1
-                }
-                if (O && !j) return y || (y = new n), _ || l(t) ? i(t, e, r, v, g, y) : o(t, e, m, r, v, g, y);
-                if (!(1 & r)) {
-                    var S = j && d.call(t, "__wrapped__"),
-                        E = w && d.call(e, "__wrapped__");
-                    if (S || E) {
-                        var A = S ? t.value() : t,
-                            k = E ? e.value() : e;
-                        return y || (y = new n), g(A, k, r, v, y)
+                if (t > o) throw new RangeError('The value "' + t + '" is invalid for option "size"');
+                var e = new Uint8Array(t);
+                return e.__proto__ = c.prototype, e
+            }
+
+            function c(t, e, r) {
+                if ("number" == typeof t) {
+                    if ("string" == typeof e) throw new TypeError('The "string" argument must be of type string. Received type number');
+                    return h(t)
+                }
+                return a(t, e, r)
+            }
+
+            function a(t, e, r) {
+                if ("string" == typeof t) return function(t, e) {
+                    if ("string" == typeof e && "" !== e || (e = "utf8"), !c.isEncoding(e)) throw new TypeError("Unknown encoding: " + e);
+                    var r = 0 | d(t, e),
+                        n = s(r),
+                        i = n.write(t, e);
+                    return i !== r && (n = n.slice(0, i)), n
+                }(t, e);
+                if (ArrayBuffer.isView(t)) return l(t);
+                if (null == t) throw TypeError("The first argument must be one of type string, Buffer, ArrayBuffer, Array, or Array-like Object. Received type " + typeof t);
+                if (G(t, ArrayBuffer) || t && G(t.buffer, ArrayBuffer)) return function(t, e, r) {
+                    if (e < 0 || t.byteLength < e) throw new RangeError('"offset" is outside of buffer bounds');
+                    if (t.byteLength < e + (r || 0)) throw new RangeError('"length" is outside of buffer bounds');
+                    var n;
+                    return (n = void 0 === e && void 0 === r ? new Uint8Array(t) : void 0 === r ? new Uint8Array(t, e) : new Uint8Array(t, e, r)).__proto__ = c.prototype, n
+                }(t, e, r);
+                if ("number" == typeof t) throw new TypeError('The "value" argument must not be of type number. Received type number');
+                var n = t.valueOf && t.valueOf();
+                if (null != n && n !== t) return c.from(n, e, r);
+                var i = function(t) {
+                    if (c.isBuffer(t)) {
+                        var e = 0 | p(t.length),
+                            r = s(e);
+                        return 0 === r.length || t.copy(r, 0, 0, e), r
+                    }
+                    return void 0 !== t.length ? "number" != typeof t.length || H(t.length) ? s(0) : l(t) : "Buffer" === t.type && Array.isArray(t.data) ? l(t.data) : void 0
+                }(t);
+                if (i) return i;
+                if ("undefined" != typeof Symbol && null != Symbol.toPrimitive && "function" == typeof t[Symbol.toPrimitive]) return c.from(t[Symbol.toPrimitive]("string"), e, r);
+                throw new TypeError("The first argument must be one of type string, Buffer, ArrayBuffer, Array, or Array-like Object. Received type " + typeof t)
+            }
+
+            function f(t) {
+                if ("number" != typeof t) throw new TypeError('"size" argument must be of type number');
+                if (t < 0) throw new RangeError('The value "' + t + '" is invalid for option "size"')
+            }
+
+            function h(t) {
+                return f(t), s(t < 0 ? 0 : 0 | p(t))
+            }
+
+            function l(t) {
+                for (var e = t.length < 0 ? 0 : 0 | p(t.length), r = s(e), n = 0; n < e; n += 1) r[n] = 255 & t[n];
+                return r
+            }
+
+            function p(t) {
+                if (t >= o) throw new RangeError("Attempt to allocate Buffer larger than maximum size: 0x" + o.toString(16) + " bytes");
+                return 0 | t
+            }
+
+            function d(t, e) {
+                if (c.isBuffer(t)) return t.length;
+                if (ArrayBuffer.isView(t) || G(t, ArrayBuffer)) return t.byteLength;
+                if ("string" != typeof t) throw new TypeError('The "string" argument must be one of type string, Buffer, or ArrayBuffer. Received type ' + typeof t);
+                var r = t.length,
+                    n = arguments.length > 2 && !0 === arguments[2];
+                if (!n && 0 === r) return 0;
+                for (var i = !1;;) switch (e) {
+                    case "ascii":
+                    case "latin1":
+                    case "binary":
+                        return r;
+                    case "utf8":
+                    case "utf-8":
+                        return F(t).length;
+                    case "ucs2":
+                    case "ucs-2":
+                    case "utf16le":
+                    case "utf-16le":
+                        return 2 * r;
+                    case "hex":
+                        return r >>> 1;
+                    case "base64":
+                        return N(t).length;
+                    default:
+                        if (i) return n ? -1 : F(t).length;
+                        e = ("" + e).toLowerCase(), i = !0
+                }
+            }
+
+            function v(t, e, r) {
+                var n = !1;
+                if ((void 0 === e || e < 0) && (e = 0), e > this.length) return "";
+                if ((void 0 === r || r > this.length) && (r = this.length), r <= 0) return "";
+                if ((r >>>= 0) <= (e >>>= 0)) return "";
+                for (t || (t = "utf8");;) switch (t) {
+                    case "hex":
+                        return B(this, e, r);
+                    case "utf8":
+                    case "utf-8":
+                        return _(this, e, r);
+                    case "ascii":
+                        return D(this, e, r);
+                    case "latin1":
+                    case "binary":
+                        return S(this, e, r);
+                    case "base64":
+                        return M(this, e, r);
+                    case "ucs2":
+                    case "ucs-2":
+                    case "utf16le":
+                    case "utf-16le":
+                        return U(this, e, r);
+                    default:
+                        if (n) throw new TypeError("Unknown encoding: " + t);
+                        t = (t + "").toLowerCase(), n = !0
+                }
+            }
+
+            function y(t, e, r) {
+                var n = t[e];
+                t[e] = t[r], t[r] = n
+            }
+
+            function g(t, e, r, n, i) {
+                if (0 === t.length) return -1;
+                if ("string" == typeof r ? (n = r, r = 0) : r > 2147483647 ? r = 2147483647 : r < -2147483648 && (r = -2147483648), H(r = +r) && (r = i ? 0 : t.length - 1), r < 0 && (r = t.length + r), r >= t.length) {
+                    if (i) return -1;
+                    r = t.length - 1
+                } else if (r < 0) {
+                    if (!i) return -1;
+                    r = 0
+                }
+                if ("string" == typeof e && (e = c.from(e, n)), c.isBuffer(e)) return 0 === e.length ? -1 : b(t, e, r, n, i);
+                if ("number" == typeof e) return e &= 255, "function" == typeof Uint8Array.prototype.indexOf ? i ? Uint8Array.prototype.indexOf.call(t, e, r) : Uint8Array.prototype.lastIndexOf.call(t, e, r) : b(t, [e], r, n, i);
+                throw new TypeError("val must be string, number or Buffer")
+            }
+
+            function b(t, e, r, n, i) {
+                var o, u = 1,
+                    s = t.length,
+                    c = e.length;
+                if (void 0 !== n && ("ucs2" === (n = String(n).toLowerCase()) || "ucs-2" === n || "utf16le" === n || "utf-16le" === n)) {
+                    if (t.length < 2 || e.length < 2) return -1;
+                    u = 2, s /= 2, c /= 2, r /= 2
+                }
+
+                function a(t, e) {
+                    return 1 === u ? t[e] : t.readUInt16BE(e * u)
+                }
+                if (i) {
+                    var f = -1;
+                    for (o = r; o < s; o++)
+                        if (a(t, o) === a(e, -1 === f ? 0 : o - f)) {
+                            if (-1 === f && (f = o), o - f + 1 === c) return f * u
+                        } else - 1 !== f && (o -= o - f), f = -1
+                } else
+                    for (r + c > s && (r = s - c), o = r; o >= 0; o--) {
+                        for (var h = !0, l = 0; l < c; l++)
+                            if (a(t, o + l) !== a(e, l)) {
+                                h = !1;
+                                break
+                            } if (h) return o
                     }
-                }
-                return !!O && (y || (y = new n), s(t, e, r, v, g, y))
-            }
-        },
-        6840: (t, e, r) => {
-            var n = r(1049),
-                i = r(7394),
-                o = r(9259),
-                s = r(7035),
-                a = /^\[object .+?Constructor\]$/,
-                u = Function.prototype,
-                c = Object.prototype,
-                l = u.toString,
-                h = c.hasOwnProperty,
-                f = RegExp("^" + l.call(h).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
-            t.exports = function(t) {
-                return !(!o(t) || i(t)) && (n(t) ? f : a).test(s(t))
-            }
-        },
-        5522: (t, e, r) => {
-            var n = r(3366),
-                i = r(1158),
-                o = r(5125),
-                s = {};
-            s["[object Float32Array]"] = s["[object Float64Array]"] = s["[object Int8Array]"] = s["[object Int16Array]"] = s["[object Int32Array]"] = s["[object Uint8Array]"] = s["[object Uint8ClampedArray]"] = s["[object Uint16Array]"] = s["[object Uint32Array]"] = !0, s["[object Arguments]"] = s["[object Array]"] = s["[object ArrayBuffer]"] = s["[object Boolean]"] = s["[object DataView]"] = s["[object Date]"] = s["[object Error]"] = s["[object Function]"] = s["[object Map]"] = s["[object Number]"] = s["[object Object]"] = s["[object RegExp]"] = s["[object Set]"] = s["[object String]"] = s["[object WeakMap]"] = !1, t.exports = function(t) {
-                return o(t) && i(t.length) && !!s[n(t)]
-            }
-        },
-        6411: (t, e, r) => {
-            var n = r(6001),
-                i = r(4248),
-                o = Object.prototype.hasOwnProperty;
-            t.exports = function(t) {
-                if (!n(t)) return i(t);
-                var e = [];
-                for (var r in Object(t)) o.call(t, r) && "constructor" != r && e.push(r);
-                return e
+                return -1
             }
-        },
-        6473: t => {
-            t.exports = function(t, e) {
-                for (var r = -1, n = Array(t); ++r < t;) n[r] = e(r);
-                return n
+
+            function m(t, e, r, n) {
+                r = Number(r) || 0;
+                var i = t.length - r;
+                n ? (n = Number(n)) > i && (n = i) : n = i;
+                var o = e.length;
+                n > o / 2 && (n = o / 2);
+                for (var u = 0; u < n; ++u) {
+                    var s = parseInt(e.substr(2 * u, 2), 16);
+                    if (H(s)) return u;
+                    t[r + u] = s
+                }
+                return u
+            }
+
+            function w(t, e, r, n) {
+                return j(F(e, t.length - r), t, r, n)
+            }
+
+            function A(t, e, r, n) {
+                return j(function(t) {
+                    for (var e = [], r = 0; r < t.length; ++r) e.push(255 & t.charCodeAt(r));
+                    return e
+                }(e), t, r, n)
             }
-        },
-        7826: t => {
-            t.exports = function(t) {
-                return function(e) {
-                    return t(e)
-                }
+
+            function T(t, e, r, n) {
+                return A(t, e, r, n)
             }
-        },
-        9950: t => {
-            t.exports = function(t, e) {
-                return t.has(e)
+
+            function E(t, e, r, n) {
+                return j(N(e), t, r, n)
             }
-        },
-        4019: (t, e, r) => {
-            var n = r(7772)["__core-js_shared__"];
-            t.exports = n
-        },
-        4871: (t, e, r) => {
-            var n = r(5386),
-                i = r(7064),
-                o = r(9950);
-            t.exports = function(t, e, r, s, a, u) {
-                var c = 1 & r,
-                    l = t.length,
-                    h = e.length;
-                if (l != h && !(c && h > l)) return !1;
-                var f = u.get(t),
-                    p = u.get(e);
-                if (f && p) return f == e && p == t;
-                var d = -1,
-                    v = !0,
-                    g = 2 & r ? new n : void 0;
-                for (u.set(t, e), u.set(e, t); ++d < l;) {
-                    var y = t[d],
-                        _ = e[d];
-                    if (s) var b = c ? s(_, y, d, e, t, u) : s(y, _, d, t, e, u);
-                    if (void 0 !== b) {
-                        if (b) continue;
-                        v = !1;
-                        break
-                    }
-                    if (g) {
-                        if (!i(e, (function(t, e) {
-                                if (!o(g, e) && (y === t || a(y, t, r, s, u))) return g.push(e)
-                            }))) {
-                            v = !1;
-                            break
-                        }
-                    } else if (y !== _ && !a(y, _, r, s, u)) {
-                        v = !1;
-                        break
-                    }
-                }
-                return u.delete(t), u.delete(e), v
+
+            function C(t, e, r, n) {
+                return j(function(t, e) {
+                    for (var r, n, i, o = [], u = 0; u < t.length && !((e -= 2) < 0); ++u) n = (r = t.charCodeAt(u)) >> 8, i = r % 256, o.push(i), o.push(n);
+                    return o
+                }(e, t.length - r), t, r, n)
             }
-        },
-        1491: (t, e, r) => {
-            var n = r(857),
-                i = r(9162),
-                o = r(1225),
-                s = r(4871),
-                a = r(5179),
-                u = r(4207),
-                c = n ? n.prototype : void 0,
-                l = c ? c.valueOf : void 0;
-            t.exports = function(t, e, r, n, c, h, f) {
-                switch (r) {
-                    case "[object DataView]":
-                        if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
-                        t = t.buffer, e = e.buffer;
-                    case "[object ArrayBuffer]":
-                        return !(t.byteLength != e.byteLength || !h(new i(t), new i(e)));
-                    case "[object Boolean]":
-                    case "[object Date]":
-                    case "[object Number]":
-                        return o(+t, +e);
-                    case "[object Error]":
-                        return t.name == e.name && t.message == e.message;
-                    case "[object RegExp]":
-                    case "[object String]":
-                        return t == e + "";
-                    case "[object Map]":
-                        var p = a;
-                    case "[object Set]":
-                        var d = 1 & n;
-                        if (p || (p = u), t.size != e.size && !d) return !1;
-                        var v = f.get(t);
-                        if (v) return v == e;
-                        n |= 2, f.set(t, e);
-                        var g = s(p(t), p(e), n, c, h, f);
-                        return f.delete(t), g;
-                    case "[object Symbol]":
-                        if (l) return l.call(t) == l.call(e)
-                }
-                return !1
+
+            function M(t, e, r) {
+                return 0 === e && r === t.length ? n.fromByteArray(t) : n.fromByteArray(t.slice(e, r))
             }
-        },
-        7416: (t, e, r) => {
-            var n = r(3483),
-                i = Object.prototype.hasOwnProperty;
-            t.exports = function(t, e, r, o, s, a) {
-                var u = 1 & r,
-                    c = n(t),
-                    l = c.length;
-                if (l != n(e).length && !u) return !1;
-                for (var h = l; h--;) {
-                    var f = c[h];
-                    if (!(u ? f in e : i.call(e, f))) return !1
-                }
-                var p = a.get(t),
-                    d = a.get(e);
-                if (p && d) return p == e && d == t;
-                var v = !0;
-                a.set(t, e), a.set(e, t);
-                for (var g = u; ++h < l;) {
-                    var y = t[f = c[h]],
-                        _ = e[f];
-                    if (o) var b = u ? o(_, y, f, e, t, a) : o(y, _, f, t, e, a);
-                    if (!(void 0 === b ? y === _ || s(y, _, r, o, a) : b)) {
-                        v = !1;
-                        break
+
+            function _(t, e, r) {
+                r = Math.min(t.length, r);
+                for (var n = [], i = e; i < r;) {
+                    var o, u, s, c, a = t[i],
+                        f = null,
+                        h = a > 239 ? 4 : a > 223 ? 3 : a > 191 ? 2 : 1;
+                    if (i + h <= r) switch (h) {
+                        case 1:
+                            a < 128 && (f = a);
+                            break;
+                        case 2:
+                            128 == (192 & (o = t[i + 1])) && (c = (31 & a) << 6 | 63 & o) > 127 && (f = c);
+                            break;
+                        case 3:
+                            o = t[i + 1], u = t[i + 2], 128 == (192 & o) && 128 == (192 & u) && (c = (15 & a) << 12 | (63 & o) << 6 | 63 & u) > 2047 && (c < 55296 || c > 57343) && (f = c);
+                            break;
+                        case 4:
+                            o = t[i + 1], u = t[i + 2], s = t[i + 3], 128 == (192 & o) && 128 == (192 & u) && 128 == (192 & s) && (c = (15 & a) << 18 | (63 & o) << 12 | (63 & u) << 6 | 63 & s) > 65535 && c < 1114112 && (f = c)
                     }
-                    g || (g = "constructor" == f)
-                }
-                if (v && !g) {
-                    var m = t.constructor,
-                        x = e.constructor;
-                    m == x || !("constructor" in t) || !("constructor" in e) || "function" == typeof m && m instanceof m && "function" == typeof x && x instanceof x || (v = !1)
+                    null === f ? (f = 65533, h = 1) : f > 65535 && (f -= 65536, n.push(f >>> 10 & 1023 | 55296), f = 56320 | 1023 & f), n.push(f), i += h
                 }
-                return a.delete(t), a.delete(e), v
-            }
-        },
-        1242: (t, e, r) => {
-            var n = "object" == typeof r.g && r.g && r.g.Object === Object && r.g;
-            t.exports = n
-        },
-        3483: (t, e, r) => {
-            var n = r(1897),
-                i = r(633),
-                o = r(249);
-            t.exports = function(t) {
-                return n(t, o, i)
-            }
-        },
-        7937: (t, e, r) => {
-            var n = r(8304);
-            t.exports = function(t, e) {
-                var r = t.__data__;
-                return n(e) ? r["string" == typeof e ? "string" : "hash"] : r.map
-            }
-        },
-        8761: (t, e, r) => {
-            var n = r(6840),
-                i = r(8109);
-            t.exports = function(t, e) {
-                var r = i(t, e);
-                return n(r) ? r : void 0
+                return function(t) {
+                    var e = t.length;
+                    if (e <= I) return String.fromCharCode.apply(String, t);
+                    for (var r = "", n = 0; n < e;) r += String.fromCharCode.apply(String, t.slice(n, n += I));
+                    return r
+                }(n)
             }
-        },
-        2107: (t, e, r) => {
-            var n = r(857),
-                i = Object.prototype,
-                o = i.hasOwnProperty,
-                s = i.toString,
-                a = n ? n.toStringTag : void 0;
-            t.exports = function(t) {
-                var e = o.call(t, a),
-                    r = t[a];
+            e.kMaxLength = u, c.TYPED_ARRAY_SUPPORT = function() {
                 try {
-                    t[a] = void 0;
-                    var n = !0
-                } catch (t) {}
-                var i = s.call(t);
-                return n && (e ? t[a] = r : delete t[a]), i
-            }
-        },
-        633: (t, e, r) => {
-            var n = r(7552),
-                i = r(981),
-                o = Object.prototype.propertyIsEnumerable,
-                s = Object.getOwnPropertySymbols,
-                a = s ? function(t) {
-                    return null == t ? [] : (t = Object(t), n(s(t), (function(e) {
-                        return o.call(t, e)
-                    })))
-                } : i;
-            t.exports = a
-        },
-        940: (t, e, r) => {
-            var n = r(9515),
-                i = r(326),
-                o = r(2760),
-                s = r(2143),
-                a = r(3215),
-                u = r(3366),
-                c = r(7035),
-                l = "[object Map]",
-                h = "[object Promise]",
-                f = "[object Set]",
-                p = "[object WeakMap]",
-                d = "[object DataView]",
-                v = c(n),
-                g = c(i),
-                y = c(o),
-                _ = c(s),
-                b = c(a),
-                m = u;
-            (n && m(new n(new ArrayBuffer(1))) != d || i && m(new i) != l || o && m(o.resolve()) != h || s && m(new s) != f || a && m(new a) != p) && (m = function(t) {
-                var e = u(t),
-                    r = "[object Object]" == e ? t.constructor : void 0,
-                    n = r ? c(r) : "";
-                if (n) switch (n) {
-                    case v:
-                        return d;
-                    case g:
-                        return l;
-                    case y:
-                        return h;
-                    case _:
-                        return f;
-                    case b:
-                        return p
-                }
-                return e
-            }), t.exports = m
-        },
-        8109: t => {
-            t.exports = function(t, e) {
-                return null == t ? void 0 : t[e]
-            }
-        },
-        2118: (t, e, r) => {
-            var n = r(9191);
-            t.exports = function() {
-                this.__data__ = n ? n(null) : {}, this.size = 0
-            }
-        },
-        6909: t => {
-            t.exports = function(t) {
-                var e = this.has(t) && delete this.__data__[t];
-                return this.size -= e ? 1 : 0, e
-            }
-        },
-        8138: (t, e, r) => {
-            var n = r(9191),
-                i = Object.prototype.hasOwnProperty;
-            t.exports = function(t) {
-                var e = this.__data__;
-                if (n) {
-                    var r = e[t];
-                    return "__lodash_hash_undefined__" === r ? void 0 : r
-                }
-                return i.call(e, t) ? e[t] : void 0
-            }
-        },
-        4174: (t, e, r) => {
-            var n = r(9191),
-                i = Object.prototype.hasOwnProperty;
-            t.exports = function(t) {
-                var e = this.__data__;
-                return n ? void 0 !== e[t] : i.call(e, t)
-            }
-        },
-        7942: (t, e, r) => {
-            var n = r(9191);
-            t.exports = function(t, e) {
-                var r = this.__data__;
-                return this.size += this.has(t) ? 0 : 1, r[t] = n && void 0 === e ? "__lodash_hash_undefined__" : e, this
-            }
-        },
-        9045: t => {
-            var e = /^(?:0|[1-9]\d*)$/;
-            t.exports = function(t, r) {
-                var n = typeof t;
-                return !!(r = null == r ? 9007199254740991 : r) && ("number" == n || "symbol" != n && e.test(t)) && t > -1 && t % 1 == 0 && t < r
-            }
-        },
-        8304: t => {
-            t.exports = function(t) {
-                var e = typeof t;
-                return "string" == e || "number" == e || "symbol" == e || "boolean" == e ? "__proto__" !== t : null === t
-            }
-        },
-        7394: (t, e, r) => {
-            var n, i = r(4019),
-                o = (n = /[^.]+$/.exec(i && i.keys && i.keys.IE_PROTO || "")) ? "Symbol(src)_1." + n : "";
-            t.exports = function(t) {
-                return !!o && o in t
-            }
-        },
-        6001: t => {
-            var e = Object.prototype;
-            t.exports = function(t) {
-                var r = t && t.constructor;
-                return t === ("function" == typeof r && r.prototype || e)
-            }
-        },
-        3945: t => {
-            t.exports = function() {
-                this.__data__ = [], this.size = 0
-            }
-        },
-        1846: (t, e, r) => {
-            var n = r(2218),
-                i = Array.prototype.splice;
-            t.exports = function(t) {
-                var e = this.__data__,
-                    r = n(e, t);
-                return !(r < 0 || (r == e.length - 1 ? e.pop() : i.call(e, r, 1), --this.size, 0))
-            }
-        },
-        8028: (t, e, r) => {
-            var n = r(2218);
-            t.exports = function(t) {
-                var e = this.__data__,
-                    r = n(e, t);
-                return r < 0 ? void 0 : e[r][1]
-            }
-        },
-        2344: (t, e, r) => {
-            var n = r(2218);
-            t.exports = function(t) {
-                return n(this.__data__, t) > -1
-            }
-        },
-        4769: (t, e, r) => {
-            var n = r(2218);
-            t.exports = function(t, e) {
-                var r = this.__data__,
-                    i = n(r, t);
-                return i < 0 ? (++this.size, r.push([t, e])) : r[i][1] = e, this
-            }
-        },
-        2411: (t, e, r) => {
-            var n = r(9612),
-                i = r(235),
-                o = r(326);
-            t.exports = function() {
-                this.size = 0, this.__data__ = {
-                    hash: new n,
-                    map: new(o || i),
-                    string: new n
+                    var t = new Uint8Array(1);
+                    return t.__proto__ = {
+                        __proto__: Uint8Array.prototype,
+                        foo: function() {
+                            return 42
+                        }
+                    }, 42 === t.foo()
+                } catch (t) {
+                    return !1
                 }
-            }
-        },
-        6417: (t, e, r) => {
-            var n = r(7937);
-            t.exports = function(t) {
-                var e = n(this, t).delete(t);
-                return this.size -= e ? 1 : 0, e
-            }
-        },
-        6928: (t, e, r) => {
-            var n = r(7937);
-            t.exports = function(t) {
-                return n(this, t).get(t)
-            }
-        },
-        9493: (t, e, r) => {
-            var n = r(7937);
-            t.exports = function(t) {
-                return n(this, t).has(t)
-            }
-        },
-        4150: (t, e, r) => {
-            var n = r(7937);
-            t.exports = function(t, e) {
-                var r = n(this, t),
-                    i = r.size;
-                return r.set(t, e), this.size += r.size == i ? 0 : 1, this
-            }
-        },
-        5179: t => {
-            t.exports = function(t) {
-                var e = -1,
-                    r = Array(t.size);
-                return t.forEach((function(t, n) {
-                    r[++e] = [n, t]
-                })), r
-            }
-        },
-        9191: (t, e, r) => {
-            var n = r(8761)(Object, "create");
-            t.exports = n
-        },
-        4248: (t, e, r) => {
-            var n = r(241)(Object.keys, Object);
-            t.exports = n
-        },
-        4146: (t, e, r) => {
-            t = r.nmd(t);
-            var n = r(1242),
-                i = e && !e.nodeType && e,
-                o = i && t && !t.nodeType && t,
-                s = o && o.exports === i && n.process,
-                a = function() {
-                    try {
-                        return o && o.require && o.require("util").types || s && s.binding && s.binding("util")
-                    } catch (t) {}
-                }();
-            t.exports = a
-        },
-        7157: t => {
-            var e = Object.prototype.toString;
-            t.exports = function(t) {
-                return e.call(t)
-            }
-        },
-        241: t => {
-            t.exports = function(t, e) {
-                return function(r) {
-                    return t(e(r))
+            }(), c.TYPED_ARRAY_SUPPORT || "undefined" == typeof console || "function" != typeof console.error || console.error("This browser lacks typed array (Uint8Array) support which is required by `buffer` v5.x. Use `buffer` v4.x if you require old browser support."), Object.defineProperty(c.prototype, "parent", {
+                enumerable: !0,
+                get: function() {
+                    if (c.isBuffer(this)) return this.buffer
+                }
+            }), Object.defineProperty(c.prototype, "offset", {
+                enumerable: !0,
+                get: function() {
+                    if (c.isBuffer(this)) return this.byteOffset
+                }
+            }), e.Buffer = c, "undefined" != typeof Symbol && null != Symbol.species && c[Symbol.species] === c && Object.defineProperty(c, Symbol.species, {
+                value: null,
+                configurable: !0,
+                enumerable: !1,
+                writable: !1
+            }), c.poolSize = 8192, c.from = function(t, e, r) {
+                return a(t, e, r)
+            }, c.prototype.__proto__ = Uint8Array.prototype, c.__proto__ = Uint8Array, c.alloc = function(t, e, r) {
+                return function(t, e, r) {
+                    return f(t), t <= 0 ? s(t) : void 0 !== e ? "string" == typeof r ? s(t).fill(e, r) : s(t).fill(e) : s(t)
+                }(t, e, r)
+            }, c.allocUnsafe = function(t) {
+                return h(t)
+            }, c.allocUnsafeSlow = function(t) {
+                return h(t)
+            }, e.SlowBuffer = function(t) {
+                return +t != t && (t = 0), c.alloc(+t)
+            }, c.isBuffer = function(t) {
+                return null != t && !0 === t._isBuffer && t !== c.prototype
+            }, c.compare = function(t, e) {
+                if (G(t, Uint8Array) && (t = c.from(t, t.offset, t.byteLength)), G(e, Uint8Array) && (e = c.from(e, e.offset, e.byteLength)), !c.isBuffer(t) || !c.isBuffer(e)) throw new TypeError('The "buf1", "buf2" arguments must be one of type Buffer or Uint8Array');
+                if (t === e) return 0;
+                for (var r = t.length, n = e.length, i = 0, o = Math.min(r, n); i < o; ++i)
+                    if (t[i] !== e[i]) {
+                        r = t[i], n = e[i];
+                        break
+                    } return r < n ? -1 : n < r ? 1 : 0
+            }, c.isEncoding = function(t) {
+                switch (String(t).toLowerCase()) {
+                    case "hex":
+                    case "utf8":
+                    case "utf-8":
+                    case "ascii":
+                    case "latin1":
+                    case "binary":
+                    case "base64":
+                    case "ucs2":
+                    case "ucs-2":
+                    case "utf16le":
+                    case "utf-16le":
+                        return !0;
+                    default:
+                        return !1
+                }
+            }, c.concat = function(t, e) {
+                if (!Array.isArray(t)) throw new TypeError('"list" argument must be an Array of Buffers');
+                if (0 === t.length) return c.alloc(0);
+                var r;
+                if (void 0 === e)
+                    for (e = 0, r = 0; r < t.length; ++r) e += t[r].length;
+                var n = c.allocUnsafe(e),
+                    i = 0;
+                for (r = 0; r < t.length; ++r) {
+                    var o = t[r];
+                    if (G(o, Uint8Array) && (o = c.from(o)), !c.isBuffer(o)) throw new TypeError('"list" argument must be an Array of Buffers');
+                    o.copy(n, i), i += o.length
                 }
+                return n
+            }, c.byteLength = d, c.prototype._isBuffer = !0, c.prototype.swap16 = function() {
+                var t = this.length;
+                if (t % 2 != 0) throw new RangeError("Buffer size must be a multiple of 16-bits");
+                for (var e = 0; e < t; e += 2) y(this, e, e + 1);
+                return this
+            }, c.prototype.swap32 = function() {
+                var t = this.length;
+                if (t % 4 != 0) throw new RangeError("Buffer size must be a multiple of 32-bits");
+                for (var e = 0; e < t; e += 4) y(this, e, e + 3), y(this, e + 1, e + 2);
+                return this
+            }, c.prototype.swap64 = function() {
+                var t = this.length;
+                if (t % 8 != 0) throw new RangeError("Buffer size must be a multiple of 64-bits");
+                for (var e = 0; e < t; e += 8) y(this, e, e + 7), y(this, e + 1, e + 6), y(this, e + 2, e + 5), y(this, e + 3, e + 4);
+                return this
+            }, c.prototype.toString = function() {
+                var t = this.length;
+                return 0 === t ? "" : 0 === arguments.length ? _(this, 0, t) : v.apply(this, arguments)
+            }, c.prototype.toLocaleString = c.prototype.toString, c.prototype.equals = function(t) {
+                if (!c.isBuffer(t)) throw new TypeError("Argument must be a Buffer");
+                return this === t || 0 === c.compare(this, t)
+            }, c.prototype.inspect = function() {
+                var t = "";
+                return t = this.toString("hex", 0, 50).replace(/(.{2})/g, "$1 ").trim(), this.length > 50 && (t += " ... "), "<Buffer " + t + ">"
+            }, c.prototype.compare = function(t, e, r, n, i) {
+                if (G(t, Uint8Array) && (t = c.from(t, t.offset, t.byteLength)), !c.isBuffer(t)) throw new TypeError('The "target" argument must be one of type Buffer or Uint8Array. Received type ' + typeof t);
+                if (void 0 === e && (e = 0), void 0 === r && (r = t ? t.length : 0), void 0 === n && (n = 0), void 0 === i && (i = this.length), e < 0 || r > t.length || n < 0 || i > this.length) throw new RangeError("out of range index");
+                if (n >= i && e >= r) return 0;
+                if (n >= i) return -1;
+                if (e >= r) return 1;
+                if (this === t) return 0;
+                for (var o = (i >>>= 0) - (n >>>= 0), u = (r >>>= 0) - (e >>>= 0), s = Math.min(o, u), a = this.slice(n, i), f = t.slice(e, r), h = 0; h < s; ++h)
+                    if (a[h] !== f[h]) {
+                        o = a[h], u = f[h];
+                        break
+                    } return o < u ? -1 : u < o ? 1 : 0
+            }, c.prototype.includes = function(t, e, r) {
+                return -1 !== this.indexOf(t, e, r)
+            }, c.prototype.indexOf = function(t, e, r) {
+                return g(this, t, e, r, !0)
+            }, c.prototype.lastIndexOf = function(t, e, r) {
+                return g(this, t, e, r, !1)
+            }, c.prototype.write = function(t, e, r, n) {
+                if (void 0 === e) n = "utf8", r = this.length, e = 0;
+                else if (void 0 === r && "string" == typeof e) n = e, r = this.length, e = 0;
+                else {
+                    if (!isFinite(e)) throw new Error("Buffer.write(string, encoding, offset[, length]) is no longer supported");
+                    e >>>= 0, isFinite(r) ? (r >>>= 0, void 0 === n && (n = "utf8")) : (n = r, r = void 0)
+                }
+                var i = this.length - e;
+                if ((void 0 === r || r > i) && (r = i), t.length > 0 && (r < 0 || e < 0) || e > this.length) throw new RangeError("Attempt to write outside buffer bounds");
+                n || (n = "utf8");
+                for (var o = !1;;) switch (n) {
+                    case "hex":
+                        return m(this, t, e, r);
+                    case "utf8":
+                    case "utf-8":
+                        return w(this, t, e, r);
+                    case "ascii":
+                        return A(this, t, e, r);
+                    case "latin1":
+                    case "binary":
+                        return T(this, t, e, r);
+                    case "base64":
+                        return E(this, t, e, r);
+                    case "ucs2":
+                    case "ucs-2":
+                    case "utf16le":
+                    case "utf-16le":
+                        return C(this, t, e, r);
+                    default:
+                        if (o) throw new TypeError("Unknown encoding: " + n);
+                        n = ("" + n).toLowerCase(), o = !0
+                }
+            }, c.prototype.toJSON = function() {
+                return {
+                    type: "Buffer",
+                    data: Array.prototype.slice.call(this._arr || this, 0)
+                }
+            };
+            var I = 4096;
+
+            function D(t, e, r) {
+                var n = "";
+                r = Math.min(t.length, r);
+                for (var i = e; i < r; ++i) n += String.fromCharCode(127 & t[i]);
+                return n
             }
-        },
-        7772: (t, e, r) => {
-            var n = r(1242),
-                i = "object" == typeof self && self && self.Object === Object && self,
-                o = n || i || Function("return this")();
-            t.exports = o
-        },
-        2842: t => {
-            t.exports = function(t) {
-                return this.__data__.set(t, "__lodash_hash_undefined__"), this
+
+            function S(t, e, r) {
+                var n = "";
+                r = Math.min(t.length, r);
+                for (var i = e; i < r; ++i) n += String.fromCharCode(t[i]);
+                return n
             }
-        },
-        2482: t => {
-            t.exports = function(t) {
-                return this.__data__.has(t)
+
+            function B(t, e, r) {
+                var n, i = t.length;
+                (!e || e < 0) && (e = 0), (!r || r < 0 || r > i) && (r = i);
+                for (var o = "", u = e; u < r; ++u) o += (n = t[u]) < 16 ? "0" + n.toString(16) : n.toString(16);
+                return o
             }
-        },
-        4207: t => {
-            t.exports = function(t) {
-                var e = -1,
-                    r = Array(t.size);
-                return t.forEach((function(t) {
-                    r[++e] = t
-                })), r
+
+            function U(t, e, r) {
+                for (var n = t.slice(e, r), i = "", o = 0; o < n.length; o += 2) i += String.fromCharCode(n[o] + 256 * n[o + 1]);
+                return i
             }
-        },
-        5243: (t, e, r) => {
-            var n = r(235);
-            t.exports = function() {
-                this.__data__ = new n, this.size = 0
+
+            function k(t, e, r) {
+                if (t % 1 != 0 || t < 0) throw new RangeError("offset is not uint");
+                if (t + e > r) throw new RangeError("Trying to access beyond buffer length")
             }
-        },
-        2858: t => {
-            t.exports = function(t) {
-                var e = this.__data__,
-                    r = e.delete(t);
-                return this.size = e.size, r
+
+            function O(t, e, r, n, i, o) {
+                if (!c.isBuffer(t)) throw new TypeError('"buffer" argument must be a Buffer instance');
+                if (e > i || e < o) throw new RangeError('"value" argument is out of bounds');
+                if (r + n > t.length) throw new RangeError("Index out of range")
             }
-        },
-        4417: t => {
-            t.exports = function(t) {
-                return this.__data__.get(t)
+
+            function L(t, e, r, n, i, o) {
+                if (r + n > t.length) throw new RangeError("Index out of range");
+                if (r < 0) throw new RangeError("Index out of range")
             }
-        },
-        8605: t => {
-            t.exports = function(t) {
-                return this.__data__.has(t)
+
+            function R(t, e, r, n, o) {
+                return e = +e, r >>>= 0, o || L(t, 0, r, 4), i.write(t, e, r, n, 23, 4), r + 4
             }
-        },
-        1418: (t, e, r) => {
-            var n = r(235),
-                i = r(326),
-                o = r(6738);
-            t.exports = function(t, e) {
-                var r = this.__data__;
-                if (r instanceof n) {
-                    var s = r.__data__;
-                    if (!i || s.length < 199) return s.push([t, e]), this.size = ++r.size, this;
-                    r = this.__data__ = new o(s)
-                }
-                return r.set(t, e), this.size = r.size, this
+
+            function x(t, e, r, n, o) {
+                return e = +e, r >>>= 0, o || L(t, 0, r, 8), i.write(t, e, r, n, 52, 8), r + 8
             }
-        },
-        7035: t => {
-            var e = Function.prototype.toString;
-            t.exports = function(t) {
-                if (null != t) {
-                    try {
-                        return e.call(t)
-                    } catch (t) {}
-                    try {
-                        return t + ""
-                    } catch (t) {}
+            c.prototype.slice = function(t, e) {
+                var r = this.length;
+                (t = ~~t) < 0 ? (t += r) < 0 && (t = 0) : t > r && (t = r), (e = void 0 === e ? r : ~~e) < 0 ? (e += r) < 0 && (e = 0) : e > r && (e = r), e < t && (e = t);
+                var n = this.subarray(t, e);
+                return n.__proto__ = c.prototype, n
+            }, c.prototype.readUIntLE = function(t, e, r) {
+                t >>>= 0, e >>>= 0, r || k(t, e, this.length);
+                for (var n = this[t], i = 1, o = 0; ++o < e && (i *= 256);) n += this[t + o] * i;
+                return n
+            }, c.prototype.readUIntBE = function(t, e, r) {
+                t >>>= 0, e >>>= 0, r || k(t, e, this.length);
+                for (var n = this[t + --e], i = 1; e > 0 && (i *= 256);) n += this[t + --e] * i;
+                return n
+            }, c.prototype.readUInt8 = function(t, e) {
+                return t >>>= 0, e || k(t, 1, this.length), this[t]
+            }, c.prototype.readUInt16LE = function(t, e) {
+                return t >>>= 0, e || k(t, 2, this.length), this[t] | this[t + 1] << 8
+            }, c.prototype.readUInt16BE = function(t, e) {
+                return t >>>= 0, e || k(t, 2, this.length), this[t] << 8 | this[t + 1]
+            }, c.prototype.readUInt32LE = function(t, e) {
+                return t >>>= 0, e || k(t, 4, this.length), (this[t] | this[t + 1] << 8 | this[t + 2] << 16) + 16777216 * this[t + 3]
+            }, c.prototype.readUInt32BE = function(t, e) {
+                return t >>>= 0, e || k(t, 4, this.length), 16777216 * this[t] + (this[t + 1] << 16 | this[t + 2] << 8 | this[t + 3])
+            }, c.prototype.readIntLE = function(t, e, r) {
+                t >>>= 0, e >>>= 0, r || k(t, e, this.length);
+                for (var n = this[t], i = 1, o = 0; ++o < e && (i *= 256);) n += this[t + o] * i;
+                return n >= (i *= 128) && (n -= Math.pow(2, 8 * e)), n
+            }, c.prototype.readIntBE = function(t, e, r) {
+                t >>>= 0, e >>>= 0, r || k(t, e, this.length);
+                for (var n = e, i = 1, o = this[t + --n]; n > 0 && (i *= 256);) o += this[t + --n] * i;
+                return o >= (i *= 128) && (o -= Math.pow(2, 8 * e)), o
+            }, c.prototype.readInt8 = function(t, e) {
+                return t >>>= 0, e || k(t, 1, this.length), 128 & this[t] ? -1 * (255 - this[t] + 1) : this[t]
+            }, c.prototype.readInt16LE = function(t, e) {
+                t >>>= 0, e || k(t, 2, this.length);
+                var r = this[t] | this[t + 1] << 8;
+                return 32768 & r ? 4294901760 | r : r
+            }, c.prototype.readInt16BE = function(t, e) {
+                t >>>= 0, e || k(t, 2, this.length);
+                var r = this[t + 1] | this[t] << 8;
+                return 32768 & r ? 4294901760 | r : r
+            }, c.prototype.readInt32LE = function(t, e) {
+                return t >>>= 0, e || k(t, 4, this.length), this[t] | this[t + 1] << 8 | this[t + 2] << 16 | this[t + 3] << 24
+            }, c.prototype.readInt32BE = function(t, e) {
+                return t >>>= 0, e || k(t, 4, this.length), this[t] << 24 | this[t + 1] << 16 | this[t + 2] << 8 | this[t + 3]
+            }, c.prototype.readFloatLE = function(t, e) {
+                return t >>>= 0, e || k(t, 4, this.length), i.read(this, t, !0, 23, 4)
+            }, c.prototype.readFloatBE = function(t, e) {
+                return t >>>= 0, e || k(t, 4, this.length), i.read(this, t, !1, 23, 4)
+            }, c.prototype.readDoubleLE = function(t, e) {
+                return t >>>= 0, e || k(t, 8, this.length), i.read(this, t, !0, 52, 8)
+            }, c.prototype.readDoubleBE = function(t, e) {
+                return t >>>= 0, e || k(t, 8, this.length), i.read(this, t, !1, 52, 8)
+            }, c.prototype.writeUIntLE = function(t, e, r, n) {
+                t = +t, e >>>= 0, r >>>= 0, n || O(this, t, e, r, Math.pow(2, 8 * r) - 1, 0);
+                var i = 1,
+                    o = 0;
+                for (this[e] = 255 & t; ++o < r && (i *= 256);) this[e + o] = t / i & 255;
+                return e + r
+            }, c.prototype.writeUIntBE = function(t, e, r, n) {
+                t = +t, e >>>= 0, r >>>= 0, n || O(this, t, e, r, Math.pow(2, 8 * r) - 1, 0);
+                var i = r - 1,
+                    o = 1;
+                for (this[e + i] = 255 & t; --i >= 0 && (o *= 256);) this[e + i] = t / o & 255;
+                return e + r
+            }, c.prototype.writeUInt8 = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 1, 255, 0), this[e] = 255 & t, e + 1
+            }, c.prototype.writeUInt16LE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 2, 65535, 0), this[e] = 255 & t, this[e + 1] = t >>> 8, e + 2
+            }, c.prototype.writeUInt16BE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 2, 65535, 0), this[e] = t >>> 8, this[e + 1] = 255 & t, e + 2
+            }, c.prototype.writeUInt32LE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 4, 4294967295, 0), this[e + 3] = t >>> 24, this[e + 2] = t >>> 16, this[e + 1] = t >>> 8, this[e] = 255 & t, e + 4
+            }, c.prototype.writeUInt32BE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 4, 4294967295, 0), this[e] = t >>> 24, this[e + 1] = t >>> 16, this[e + 2] = t >>> 8, this[e + 3] = 255 & t, e + 4
+            }, c.prototype.writeIntLE = function(t, e, r, n) {
+                if (t = +t, e >>>= 0, !n) {
+                    var i = Math.pow(2, 8 * r - 1);
+                    O(this, t, e, r, i - 1, -i)
+                }
+                var o = 0,
+                    u = 1,
+                    s = 0;
+                for (this[e] = 255 & t; ++o < r && (u *= 256);) t < 0 && 0 === s && 0 !== this[e + o - 1] && (s = 1), this[e + o] = (t / u >> 0) - s & 255;
+                return e + r
+            }, c.prototype.writeIntBE = function(t, e, r, n) {
+                if (t = +t, e >>>= 0, !n) {
+                    var i = Math.pow(2, 8 * r - 1);
+                    O(this, t, e, r, i - 1, -i)
+                }
+                var o = r - 1,
+                    u = 1,
+                    s = 0;
+                for (this[e + o] = 255 & t; --o >= 0 && (u *= 256);) t < 0 && 0 === s && 0 !== this[e + o + 1] && (s = 1), this[e + o] = (t / u >> 0) - s & 255;
+                return e + r
+            }, c.prototype.writeInt8 = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 1, 127, -128), t < 0 && (t = 255 + t + 1), this[e] = 255 & t, e + 1
+            }, c.prototype.writeInt16LE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 2, 32767, -32768), this[e] = 255 & t, this[e + 1] = t >>> 8, e + 2
+            }, c.prototype.writeInt16BE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 2, 32767, -32768), this[e] = t >>> 8, this[e + 1] = 255 & t, e + 2
+            }, c.prototype.writeInt32LE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 4, 2147483647, -2147483648), this[e] = 255 & t, this[e + 1] = t >>> 8, this[e + 2] = t >>> 16, this[e + 3] = t >>> 24, e + 4
+            }, c.prototype.writeInt32BE = function(t, e, r) {
+                return t = +t, e >>>= 0, r || O(this, t, e, 4, 2147483647, -2147483648), t < 0 && (t = 4294967295 + t + 1), this[e] = t >>> 24, this[e + 1] = t >>> 16, this[e + 2] = t >>> 8, this[e + 3] = 255 & t, e + 4
+            }, c.prototype.writeFloatLE = function(t, e, r) {
+                return R(this, t, e, !0, r)
+            }, c.prototype.writeFloatBE = function(t, e, r) {
+                return R(this, t, e, !1, r)
+            }, c.prototype.writeDoubleLE = function(t, e, r) {
+                return x(this, t, e, !0, r)
+            }, c.prototype.writeDoubleBE = function(t, e, r) {
+                return x(this, t, e, !1, r)
+            }, c.prototype.copy = function(t, e, r, n) {
+                if (!c.isBuffer(t)) throw new TypeError("argument should be a Buffer");
+                if (r || (r = 0), n || 0 === n || (n = this.length), e >= t.length && (e = t.length), e || (e = 0), n > 0 && n < r && (n = r), n === r) return 0;
+                if (0 === t.length || 0 === this.length) return 0;
+                if (e < 0) throw new RangeError("targetStart out of bounds");
+                if (r < 0 || r >= this.length) throw new RangeError("Index out of range");
+                if (n < 0) throw new RangeError("sourceEnd out of bounds");
+                n > this.length && (n = this.length), t.length - e < n - r && (n = t.length - e + r);
+                var i = n - r;
+                if (this === t && "function" == typeof Uint8Array.prototype.copyWithin) this.copyWithin(e, r, n);
+                else if (this === t && r < e && e < n)
+                    for (var o = i - 1; o >= 0; --o) t[o + e] = this[o + r];
+                else Uint8Array.prototype.set.call(t, this.subarray(r, n), e);
+                return i
+            }, c.prototype.fill = function(t, e, r, n) {
+                if ("string" == typeof t) {
+                    if ("string" == typeof e ? (n = e, e = 0, r = this.length) : "string" == typeof r && (n = r, r = this.length), void 0 !== n && "string" != typeof n) throw new TypeError("encoding must be a string");
+                    if ("string" == typeof n && !c.isEncoding(n)) throw new TypeError("Unknown encoding: " + n);
+                    if (1 === t.length) {
+                        var i = t.charCodeAt(0);
+                        ("utf8" === n && i < 128 || "latin1" === n) && (t = i)
+                    }
+                } else "number" == typeof t && (t &= 255);
+                if (e < 0 || this.length < e || this.length < r) throw new RangeError("Out of range index");
+                if (r <= e) return this;
+                var o;
+                if (e >>>= 0, r = void 0 === r ? this.length : r >>> 0, t || (t = 0), "number" == typeof t)
+                    for (o = e; o < r; ++o) this[o] = t;
+                else {
+                    var u = c.isBuffer(t) ? t : c.from(t, n),
+                        s = u.length;
+                    if (0 === s) throw new TypeError('The value "' + t + '" is invalid for argument "value"');
+                    for (o = 0; o < r - e; ++o) this[o + e] = u[o % s]
+                }
+                return this
+            };
+            var P = /[^+/0-9A-Za-z-_]/g;
+
+            function F(t, e) {
+                var r;
+                e = e || 1 / 0;
+                for (var n = t.length, i = null, o = [], u = 0; u < n; ++u) {
+                    if ((r = t.charCodeAt(u)) > 55295 && r < 57344) {
+                        if (!i) {
+                            if (r > 56319) {
+                                (e -= 3) > -1 && o.push(239, 191, 189);
+                                continue
+                            }
+                            if (u + 1 === n) {
+                                (e -= 3) > -1 && o.push(239, 191, 189);
+                                continue
+                            }
+                            i = r;
+                            continue
+                        }
+                        if (r < 56320) {
+                            (e -= 3) > -1 && o.push(239, 191, 189), i = r;
+                            continue
+                        }
+                        r = 65536 + (i - 55296 << 10 | r - 56320)
+                    } else i && (e -= 3) > -1 && o.push(239, 191, 189);
+                    if (i = null, r < 128) {
+                        if ((e -= 1) < 0) break;
+                        o.push(r)
+                    } else if (r < 2048) {
+                        if ((e -= 2) < 0) break;
+                        o.push(r >> 6 | 192, 63 & r | 128)
+                    } else if (r < 65536) {
+                        if ((e -= 3) < 0) break;
+                        o.push(r >> 12 | 224, r >> 6 & 63 | 128, 63 & r | 128)
+                    } else {
+                        if (!(r < 1114112)) throw new Error("Invalid code point");
+                        if ((e -= 4) < 0) break;
+                        o.push(r >> 18 | 240, r >> 12 & 63 | 128, r >> 6 & 63 | 128, 63 & r | 128)
+                    }
                 }
-                return ""
-            }
-        },
-        1225: t => {
-            t.exports = function(t, e) {
-                return t === e || t != t && e != e
-            }
-        },
-        9631: (t, e, r) => {
-            var n = r(5183),
-                i = r(5125),
-                o = Object.prototype,
-                s = o.hasOwnProperty,
-                a = o.propertyIsEnumerable,
-                u = n(function() {
-                    return arguments
-                }()) ? n : function(t) {
-                    return i(t) && s.call(t, "callee") && !a.call(t, "callee")
-                };
-            t.exports = u
-        },
-        6152: t => {
-            var e = Array.isArray;
-            t.exports = e
-        },
-        7878: (t, e, r) => {
-            var n = r(1049),
-                i = r(1158);
-            t.exports = function(t) {
-                return null != t && i(t.length) && !n(t)
-            }
-        },
-        3226: (t, e, r) => {
-            t = r.nmd(t);
-            var n = r(7772),
-                i = r(6330),
-                o = e && !e.nodeType && e,
-                s = o && t && !t.nodeType && t,
-                a = s && s.exports === o ? n.Buffer : void 0,
-                u = (a ? a.isBuffer : void 0) || i;
-            t.exports = u
-        },
-        8149: (t, e, r) => {
-            var n = r(8746);
-            t.exports = function(t, e) {
-                return n(t, e)
-            }
-        },
-        1049: (t, e, r) => {
-            var n = r(3366),
-                i = r(9259);
-            t.exports = function(t) {
-                if (!i(t)) return !1;
-                var e = n(t);
-                return "[object Function]" == e || "[object GeneratorFunction]" == e || "[object AsyncFunction]" == e || "[object Proxy]" == e
-            }
-        },
-        1158: t => {
-            t.exports = function(t) {
-                return "number" == typeof t && t > -1 && t % 1 == 0 && t <= 9007199254740991
-            }
-        },
-        9259: t => {
-            t.exports = function(t) {
-                var e = typeof t;
-                return null != t && ("object" == e || "function" == e)
+                return o
             }
-        },
-        5125: t => {
-            t.exports = function(t) {
-                return null != t && "object" == typeof t
+
+            function N(t) {
+                return n.toByteArray(function(t) {
+                    if ((t = (t = t.split("=")[0]).trim().replace(P, "")).length < 2) return "";
+                    for (; t.length % 4 != 0;) t += "=";
+                    return t
+                }(t))
             }
-        },
-        7598: (t, e, r) => {
-            var n = r(5522),
-                i = r(7826),
-                o = r(4146),
-                s = o && o.isTypedArray,
-                a = s ? i(s) : n;
-            t.exports = a
-        },
-        249: (t, e, r) => {
-            var n = r(1634),
-                i = r(6411),
-                o = r(7878);
-            t.exports = function(t) {
-                return o(t) ? n(t) : i(t)
+
+            function j(t, e, r, n) {
+                for (var i = 0; i < n && !(i + r >= e.length || i >= t.length); ++i) e[i + r] = t[i];
+                return i
             }
-        },
-        981: t => {
-            t.exports = function() {
-                return []
+
+            function G(t, e) {
+                return t instanceof e || null != t && null != t.constructor && null != t.constructor.name && t.constructor.name === e.name
             }
-        },
-        6330: t => {
-            t.exports = function() {
-                return !1
+
+            function H(t) {
+                return t != t
             }
         },
-        3506: function(t, e, r) {
-            t.exports = function() {
-                var t = "1.13.2",
-                    e = "object" == typeof self && self.self === self && self || "object" == typeof r.g && r.g.global === r.g && r.g || Function("return this")() || {},
-                    n = Array.prototype,
-                    i = Object.prototype,
-                    o = "undefined" != typeof Symbol ? Symbol.prototype : null,
-                    s = n.push,
-                    a = n.slice,
-                    u = i.toString,
-                    c = i.hasOwnProperty,
-                    l = "undefined" != typeof ArrayBuffer,
-                    h = "undefined" != typeof DataView,
-                    f = Array.isArray,
-                    p = Object.keys,
-                    d = Object.create,
-                    v = l && ArrayBuffer.isView,
-                    g = isNaN,
-                    y = isFinite,
-                    _ = !{
-                        toString: null
-                    }.propertyIsEnumerable("toString"),
-                    b = ["valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
-                    m = Math.pow(2, 53) - 1;
-
-                function x(t, e) {
-                    return e = null == e ? t.length - 1 : +e,
+        538: function(t, e) {
+            var r = this && this.__spreadArrays || function() {
+                for (var t = 0, e = 0, r = arguments.length; e < r; e++) t += arguments[e].length;
+                var n = Array(t),
+                    i = 0;
+                for (e = 0; e < r; e++)
+                    for (var o = arguments[e], u = 0, s = o.length; u < s; u++, i++) n[i] = o[u];
+                return n
+            };
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.EventEmitter = void 0;
+            var n = function() {
+                function t() {
+                    this.events = {}
+                }
+                return t.prototype.on = function(t, e) {
+                    var r = this;
+                    return "object" != typeof this.events[t] && (this.events[t] = []), this.events[t].push(e),
                         function() {
-                            for (var r = Math.max(arguments.length - e, 0), n = Array(r), i = 0; i < r; i++) n[i] = arguments[i + e];
-                            switch (e) {
-                                case 0:
-                                    return t.call(this, n);
-                                case 1:
-                                    return t.call(this, arguments[0], n);
-                                case 2:
-                                    return t.call(this, arguments[0], arguments[1], n)
-                            }
-                            var o = Array(e + 1);
-                            for (i = 0; i < e; i++) o[i] = arguments[i];
-                            return o[e] = n, t.apply(this, o)
+                            return r.removeListener(t, e)
                         }
-                }
-
-                function j(t) {
-                    var e = typeof t;
-                    return "function" === e || "object" === e && !!t
-                }
-
-                function w(t) {
-                    return void 0 === t
-                }
-
-                function O(t) {
-                    return !0 === t || !1 === t || "[object Boolean]" === u.call(t)
-                }
-
-                function S(t) {
-                    var e = "[object " + t + "]";
-                    return function(t) {
-                        return u.call(t) === e
-                    }
-                }
-                var E = S("String"),
-                    A = S("Number"),
-                    k = S("Date"),
-                    I = S("RegExp"),
-                    T = S("Error"),
-                    P = S("Symbol"),
-                    M = S("ArrayBuffer"),
-                    z = S("Function"),
-                    N = e.document && e.document.childNodes;
-                "object" != typeof Int8Array && "function" != typeof N && (z = function(t) {
-                    return "function" == typeof t || !1
-                });
-                var $ = z,
-                    R = S("Object"),
-                    B = h && R(new DataView(new ArrayBuffer(8))),
-                    C = "undefined" != typeof Map && R(new Map),
-                    U = S("DataView"),
-                    F = B ? function(t) {
-                        return null != t && $(t.getInt8) && M(t.buffer)
-                    } : U,
-                    H = f || S("Array");
-
-                function D(t, e) {
-                    return null != t && c.call(t, e)
-                }
-                var L = S("Arguments");
-                ! function() {
-                    L(arguments) || (L = function(t) {
-                        return D(t, "callee")
-                    })
+                }, t.prototype.removeListener = function(t, e) {
+                    if ("object" == typeof this.events[t]) {
+                        var r = this.events[t].indexOf(e);
+                        r > -1 && this.events[t].splice(r, 1)
+                    }
+                }, t.prototype.removeAllListeners = function() {
+                    var t = this;
+                    Object.keys(this.events).forEach((function(e) {
+                        return t.events[e].splice(0, t.events[e].length)
+                    }))
+                }, t.prototype.emit = function(t) {
+                    for (var e = this, n = [], i = 1; i < arguments.length; i++) n[i - 1] = arguments[i];
+                    "object" == typeof this.events[t] && r(this.events[t]).forEach((function(t) {
+                        return t.apply(e, n)
+                    }))
+                }, t.prototype.once = function(t, e) {
+                    var r = this,
+                        n = this.on(t, (function() {
+                            for (var t = [], i = 0; i < arguments.length; i++) t[i] = arguments[i];
+                            n(), e.apply(r, t)
+                        }));
+                    return n
+                }, t
+            }();
+            e.EventEmitter = n
+        },
+        80: (t, e, r) => {
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.Hub = void 0;
+            var n = r(538),
+                i = r(67),
+                o = function() {
+                    function t(t) {
+                        this.emitter = new n.EventEmitter, this.autoSubscribe = !0, this.writeCue = [], this.isWriting = !1, this.bluetooth = t, this.log = console.log, this.autoSubscribe = !0, this.ports = {}, this.num2type = {
+                            23: "LED",
+                            37: "DISTANCE",
+                            38: "IMOTOR",
+                            39: "MOTOR",
+                            40: "TILT"
+                        }, this.port2num = {
+                            A: 0,
+                            B: 1,
+                            C: 2,
+                            D: 3,
+                            AB: 16,
+                            LED: 50,
+                            TILT: 58
+                        }, this.num2port = Object.entries(this.port2num).reduce((function(t, e) {
+                            var r = e[0];
+                            return t[e[1]] = r, t
+                        }), {}), this.num2action = {
+                            1: "start",
+                            5: "conflict",
+                            10: "stop"
+                        }, this.num2color = {
+                            0: "black",
+                            3: "blue",
+                            5: "green",
+                            7: "yellow",
+                            9: "red",
+                            10: "white"
+                        }, this.ledColors = ["off", "pink", "purple", "blue", "lightblue", "cyan", "green", "yellow", "orange", "red", "white"], this.addListeners()
+                    }
+                    return t.prototype.emit = function(t, e) {
+                        void 0 === e && (e = null), this.emitter.emit(t, e)
+                    }, t.prototype.addListeners = function() {
+                        var t = this;
+                        this.bluetooth.addEventListener("characteristicvaluechanged", (function(e) {
+                            var r = i.Buffer.from(e.target.value.buffer);
+                            t.parseMessage(r)
+                        })), setTimeout((function() {
+                            t.bluetooth.startNotifications()
+                        }), 1e3)
+                    }, t.prototype.parseMessage = function(t) {
+                        var e = this;
+                        if (this.num2port[t[3]]) switch (t[2]) {
+                            case 4:
+                                clearTimeout(this.portInfoTimeout), this.portInfoTimeout = setTimeout((function() {
+                                    e.autoSubscribe && e.subscribeAll(), e.connected || (e.connected = !0, e.emit("connect"))
+                                }), 1e3), this.log("Found: " + this.num2type[t[5]]), this.logDebug("Found", t), 1 === t[4] ? this.ports[t[3]] = {
+                                    type: "port",
+                                    deviceType: this.num2type[t[5]],
+                                    deviceTypeNum: t[5]
+                                } : 2 === t[4] && (this.ports[t[3]] = {
+                                    type: "group",
+                                    deviceType: this.num2type[t[5]],
+                                    deviceTypeNum: t[5],
+                                    members: [t[7], t[8]]
+                                });
+                                break;
+                            case 5:
+                                this.log("Malformed message!"), this.log("<", t);
+                                break;
+                            case 69:
+                                this.parseSensor(t);
+                                break;
+                            case 71:
+                                break;
+                            case 130:
+                                this.emit("port", {
+                                    port: this.num2port[t[3]],
+                                    action: this.num2action[t[4]]
+                                });
+                                break;
+                            default:
+                                this.log("unknown message type 0x" + t[2].toString(16)), this.log("<", t)
+                        } else this.log("parseSensor unknown port 0x" + t[3].toString(16))
+                    }, t.prototype.parseSensor = function(t) {
+                        if (this.ports[t[3]]) switch (this.ports[t[3]].deviceType) {
+                            case "DISTANCE":
+                                this.emit("color", this.num2color[t[4]]);
+                                var e;
+                                e = t[7] > 0 && t[5] < 2 ? Math.floor(20 - 2.85 * t[7]) : t[5] > 9 ? 1 / 0 : Math.floor(20 + 18 * t[5]), this.emit("distance", e);
+                                break;
+                            case "TILT":
+                                var r = t.readInt8(4),
+                                    n = t.readInt8(5);
+                                this.emit("tilt", {
+                                    roll: r,
+                                    pitch: n
+                                });
+                                break;
+                            case "MOTOR":
+                            case "IMOTOR":
+                                var i = t.readInt32LE(4);
+                                this.emit("rotation", {
+                                    port: this.num2port[t[3]],
+                                    angle: i
+                                });
+                                break;
+                            default:
+                                this.log("unknown sensor type 0x" + t[3].toString(16), t[3], this.ports[t[3]].deviceType)
+                        } else this.log("parseSensor unknown port 0x" + t[3].toString(16))
+                    }, t.prototype.setDisconnected = function() {
+                        this.connected = !1, this.noReconnect = !0, this.writeCue = []
+                    }, t.prototype.motorTime = function(t, e, r, n) {
+                        "function" == typeof r && (n = r, r = 100);
+                        var i = "string" == typeof t ? this.port2num[t] : t;
+                        this.write(this.encodeMotorTime(i, e, r), n)
+                    }, t.prototype.motorTimeMulti = function(t, e, r, n) {
+                        this.write(this.encodeMotorTimeMulti(this.port2num.AB, t, e, r), n)
+                    }, t.prototype.motorAngle = function(t, e, r, n) {
+                        "function" == typeof r && (n = r, r = 100);
+                        var i = "string" == typeof t ? this.port2num[t] : t;
+                        this.write(this.encodeMotorAngle(i, e, r), n)
+                    }, t.prototype.motorAngleMulti = function(t, e, r, n) {
+                        this.write(this.encodeMotorAngleMulti(this.port2num.AB, t, e, r), n)
+                    }, t.prototype.rawCommand = function(t, e) {
+                        var r = i.Buffer.from([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]);
+                        for (var n in t) r.writeIntLE(t[n], n);
+                        this.write(r, e)
+                    }, t.prototype.motorPowerCommand = function(t, e) {
+                        this.write(this.encodeMotorPower(t, e))
+                    }, t.prototype.encodeMotorPower = function(t, e) {
+                        void 0 === e && (e = 100);
+                        var r = "string" == typeof t ? this.port2num[t] : t,
+                            n = i.Buffer.from([9, 0, 129, r, 17, 7, 0, 100, 3]);
+                        return n.writeInt8(e, 6), n
+                    }, t.prototype.led = function(t, e) {
+                        this.write(this.encodeLed(t), e)
+                    }, t.prototype.subscribe = function(t, e, r) {
+                        void 0 === e && (e = 0), "function" == typeof e && (r = e, e = 0);
+                        var n = "string" == typeof t ? this.port2num[t] : t;
+                        this.write(i.Buffer.from([10, 0, 65, n, e, 1, 0, 0, 0, 1]), r)
+                    }, t.prototype.unsubscribe = function(t, e, r) {
+                        void 0 === e && (e = 0), "function" == typeof e && (r = e, e = 0);
+                        var n = "string" == typeof t ? this.port2num[t] : t;
+                        this.write(i.Buffer.from([10, 0, 65, n, e, 1, 0, 0, 0, 0]), r)
+                    }, t.prototype.subscribeAll = function() {
+                        var t = this;
+                        Object.entries(this.ports).forEach((function(e) {
+                            var r = e[0],
+                                n = e[1];
+                            "DISTANCE" === n.deviceType ? t.subscribe(parseInt(r, 10), 8) : "TILT" === n.deviceType ? t.subscribe(parseInt(r, 10), 0) : "IMOTOR" === n.deviceType || "MOTOR" === n.deviceType ? t.subscribe(parseInt(r, 10), 2) : t.logDebug("Port subscribtion not sent: " + r)
+                        }))
+                    }, t.prototype.write = function(t, e) {
+                        if ("string" == typeof t) {
+                            var r = [];
+                            t.split(" ").forEach((function(t) {
+                                r.push(parseInt(t, 16))
+                            })), t = i.Buffer.from(r)
+                        }
+                        this.writeCue.push({
+                            data: t,
+                            secondArg: !0,
+                            callback: e
+                        }), this.writeFromCue()
+                    }, t.prototype.writeFromCue = function() {
+                        var t = this;
+                        if (0 !== this.writeCue.length && !this.isWriting) {
+                            var e = this.writeCue.shift();
+                            this.logDebug("Writing to device", e), this.isWriting = !0, this.bluetooth.writeValue(e.data).then((function() {
+                                t.isWriting = !1, "function" == typeof e.callback && e.callback()
+                            })).catch((function(r) {
+                                t.isWriting = !1, t.log("Error while writing: " + e.data + " - Error " + r.toString())
+                            })).finally((function() {
+                                t.writeFromCue()
+                            }))
+                        }
+                    }, t.prototype.encodeMotorTimeMulti = function(t, e, r, n) {
+                        void 0 === r && (r = 100), void 0 === n && (n = -100);
+                        var o = i.Buffer.from([13, 0, 129, t, 17, 10, 0, 0, 0, 0, 100, 127, 3]);
+                        return o.writeUInt16LE(1e3 * e, 6), o.writeInt8(r, 8), o.writeInt8(n, 9), o
+                    }, t.prototype.encodeMotorTime = function(t, e, r) {
+                        void 0 === r && (r = 100);
+                        var n = i.Buffer.from([12, 0, 129, t, 17, 9, 0, 0, 0, 100, 127, 3]);
+                        return n.writeUInt16LE(1e3 * e, 6), n.writeInt8(r, 8), n
+                    }, t.prototype.encodeMotorAngleMulti = function(t, e, r, n) {
+                        void 0 === r && (r = 100), void 0 === n && (n = -100);
+                        var o = i.Buffer.from([15, 0, 129, t, 17, 12, 0, 0, 0, 0, 0, 0, 100, 127, 3]);
+                        return o.writeUInt32LE(e, 6), o.writeInt8(r, 10), o.writeInt8(n, 11), o
+                    }, t.prototype.encodeMotorAngle = function(t, e, r) {
+                        void 0 === r && (r = 100);
+                        var n = i.Buffer.from([14, 0, 129, t, 17, 11, 0, 0, 0, 0, 0, 100, 127, 3]);
+                        return n.writeUInt32LE(e, 6), n.writeInt8(r, 10), n
+                    }, t.prototype.encodeLed = function(t) {
+                        "boolean" == typeof t && (t = t ? "white" : "off");
+                        var e = "string" == typeof t ? this.ledColors.indexOf(t) : t;
+                        return i.Buffer.from([8, 0, 129, 50, 17, 81, 0, e])
+                    }, t
                 }();
-                var q = L;
-
-                function V(t) {
-                    return A(t) && g(t)
-                }
-
-                function W(t) {
-                    return function() {
-                        return t
-                    }
-                }
-
-                function J(t) {
-                    return function(e) {
-                        var r = t(e);
-                        return "number" == typeof r && r >= 0 && r <= m
-                    }
-                }
-
-                function G(t) {
-                    return function(e) {
-                        return null == e ? void 0 : e[t]
-                    }
-                }
-                var K = G("byteLength"),
-                    X = J(K),
-                    Q = /\[object ((I|Ui)nt(8|16|32)|Float(32|64)|Uint8Clamped|Big(I|Ui)nt64)Array\]/,
-                    Y = l ? function(t) {
-                        return v ? v(t) && !F(t) : X(t) && Q.test(u.call(t))
-                    } : W(!1),
-                    Z = G("length");
-
-                function tt(t, e) {
-                    e = function(t) {
-                        for (var e = {}, r = t.length, n = 0; n < r; ++n) e[t[n]] = !0;
-                        return {
-                            contains: function(t) {
-                                return !0 === e[t]
-                            },
-                            push: function(r) {
-                                return e[r] = !0, t.push(r)
+            e.Hub = o
+        },
+        382: function(t, e, r) {
+            var n, i = this && this.__extends || (n = function(t, e) {
+                    return n = Object.setPrototypeOf || {
+                        __proto__: []
+                    }
+                    instanceof Array && function(t, e) {
+                        t.__proto__ = e
+                    } || function(t, e) {
+                        for (var r in e) e.hasOwnProperty(r) && (t[r] = e[r])
+                    }, n(t, e)
+                }, function(t, e) {
+                    function r() {
+                        this.constructor = t
+                    }
+                    n(t, e), t.prototype = null === e ? Object.create(e) : (r.prototype = e.prototype, new r)
+                }),
+                o = this && this.__awaiter || function(t, e, r, n) {
+                    return new(r || (r = Promise))((function(i, o) {
+                        function u(t) {
+                            try {
+                                c(n.next(t))
+                            } catch (t) {
+                                o(t)
                             }
                         }
-                    }(e);
-                    var r = b.length,
-                        n = t.constructor,
-                        o = $(n) && n.prototype || i,
-                        s = "constructor";
-                    for (D(t, s) && !e.contains(s) && e.push(s); r--;)(s = b[r]) in t && t[s] !== o[s] && !e.contains(s) && e.push(s)
-                }
-
-                function et(t) {
-                    if (!j(t)) return [];
-                    if (p) return p(t);
-                    var e = [];
-                    for (var r in t) D(t, r) && e.push(r);
-                    return _ && tt(t, e), e
-                }
-
-                function rt(t, e) {
-                    var r = et(e),
-                        n = r.length;
-                    if (null == t) return !n;
-                    for (var i = Object(t), o = 0; o < n; o++) {
-                        var s = r[o];
-                        if (e[s] !== i[s] || !(s in i)) return !1
-                    }
-                    return !0
-                }
-
-                function nt(t) {
-                    return t instanceof nt ? t : this instanceof nt ? void(this._wrapped = t) : new nt(t)
-                }
-
-                function it(t) {
-                    return new Uint8Array(t.buffer || t, t.byteOffset || 0, K(t))
-                }
-                nt.VERSION = t, nt.prototype.value = function() {
-                    return this._wrapped
-                }, nt.prototype.valueOf = nt.prototype.toJSON = nt.prototype.value, nt.prototype.toString = function() {
-                    return String(this._wrapped)
-                };
-                var ot = "[object DataView]";
-
-                function st(t, e, r, n) {
-                    if (t === e) return 0 !== t || 1 / t == 1 / e;
-                    if (null == t || null == e) return !1;
-                    if (t != t) return e != e;
-                    var i = typeof t;
-                    return ("function" === i || "object" === i || "object" == typeof e) && function t(e, r, n, i) {
-                        e instanceof nt && (e = e._wrapped), r instanceof nt && (r = r._wrapped);
-                        var s = u.call(e);
-                        if (s !== u.call(r)) return !1;
-                        if (B && "[object Object]" == s && F(e)) {
-                            if (!F(r)) return !1;
-                            s = ot
-                        }
-                        switch (s) {
-                            case "[object RegExp]":
-                            case "[object String]":
-                                return "" + e == "" + r;
-                            case "[object Number]":
-                                return +e != +e ? +r != +r : 0 == +e ? 1 / +e == 1 / r : +e == +r;
-                            case "[object Date]":
-                            case "[object Boolean]":
-                                return +e == +r;
-                            case "[object Symbol]":
-                                return o.valueOf.call(e) === o.valueOf.call(r);
-                            case "[object ArrayBuffer]":
-                            case ot:
-                                return t(it(e), it(r), n, i)
-                        }
-                        var a = "[object Array]" === s;
-                        if (!a && Y(e)) {
-                            if (K(e) !== K(r)) return !1;
-                            if (e.buffer === r.buffer && e.byteOffset === r.byteOffset) return !0;
-                            a = !0
-                        }
-                        if (!a) {
-                            if ("object" != typeof e || "object" != typeof r) return !1;
-                            var c = e.constructor,
-                                l = r.constructor;
-                            if (c !== l && !($(c) && c instanceof c && $(l) && l instanceof l) && "constructor" in e && "constructor" in r) return !1
-                        }
-                        i = i || [];
-                        for (var h = (n = n || []).length; h--;)
-                            if (n[h] === e) return i[h] === r;
-                        if (n.push(e), i.push(r), a) {
-                            if ((h = e.length) !== r.length) return !1;
-                            for (; h--;)
-                                if (!st(e[h], r[h], n, i)) return !1
-                        } else {
-                            var f, p = et(e);
-                            if (h = p.length, et(r).length !== h) return !1;
-                            for (; h--;)
-                                if (!D(r, f = p[h]) || !st(e[f], r[f], n, i)) return !1
-                        }
-                        return n.pop(), i.pop(), !0
-                    }(t, e, r, n)
-                }
-
-                function at(t) {
-                    if (!j(t)) return [];
-                    var e = [];
-                    for (var r in t) e.push(r);
-                    return _ && tt(t, e), e
-                }
-
-                function ut(t) {
-                    var e = Z(t);
-                    return function(r) {
-                        if (null == r) return !1;
-                        var n = at(r);
-                        if (Z(n)) return !1;
-                        for (var i = 0; i < e; i++)
-                            if (!$(r[t[i]])) return !1;
-                        return t !== pt || !$(r[ct])
-                    }
-                }
-                var ct = "forEach",
-                    lt = ["clear", "delete"],
-                    ht = ["get", "has", "set"],
-                    ft = lt.concat(ct, ht),
-                    pt = lt.concat(ht),
-                    dt = ["add"].concat(lt, ct, "has"),
-                    vt = C ? ut(ft) : S("Map"),
-                    gt = C ? ut(pt) : S("WeakMap"),
-                    yt = C ? ut(dt) : S("Set"),
-                    _t = S("WeakSet");
-
-                function bt(t) {
-                    for (var e = et(t), r = e.length, n = Array(r), i = 0; i < r; i++) n[i] = t[e[i]];
-                    return n
-                }
-
-                function mt(t) {
-                    for (var e = {}, r = et(t), n = 0, i = r.length; n < i; n++) e[t[r[n]]] = r[n];
-                    return e
-                }
-
-                function xt(t) {
-                    var e = [];
-                    for (var r in t) $(t[r]) && e.push(r);
-                    return e.sort()
-                }
 
-                function jt(t, e) {
-                    return function(r) {
-                        var n = arguments.length;
-                        if (e && (r = Object(r)), n < 2 || null == r) return r;
-                        for (var i = 1; i < n; i++)
-                            for (var o = arguments[i], s = t(o), a = s.length, u = 0; u < a; u++) {
-                                var c = s[u];
-                                e && void 0 !== r[c] || (r[c] = o[c])
+                        function s(t) {
+                            try {
+                                c(n.throw(t))
+                            } catch (t) {
+                                o(t)
                             }
-                        return r
-                    }
-                }
-                var wt = jt(at),
-                    Ot = jt(et),
-                    St = jt(at, !0);
-
-                function Et(t) {
-                    if (!j(t)) return {};
-                    if (d) return d(t);
-                    var e = function() {};
-                    e.prototype = t;
-                    var r = new e;
-                    return e.prototype = null, r
-                }
-
-                function At(t) {
-                    return H(t) ? t : [t]
-                }
-
-                function kt(t) {
-                    return nt.toPath(t)
-                }
-
-                function It(t, e) {
-                    for (var r = e.length, n = 0; n < r; n++) {
-                        if (null == t) return;
-                        t = t[e[n]]
-                    }
-                    return r ? t : void 0
-                }
-
-                function Tt(t, e, r) {
-                    var n = It(t, kt(e));
-                    return w(n) ? r : n
-                }
-
-                function Pt(t) {
-                    return t
-                }
-
-                function Mt(t) {
-                    return t = Ot({}, t),
-                        function(e) {
-                            return rt(e, t)
                         }
-                }
 
-                function zt(t) {
-                    return t = kt(t),
-                        function(e) {
-                            return It(e, t)
+                        function c(t) {
+                            var e;
+                            t.done ? i(t.value) : (e = t.value, e instanceof r ? e : new r((function(t) {
+                                t(e)
+                            }))).then(u, s)
                         }
-                }
+                        c((n = n.apply(t, e || [])).next())
+                    }))
+                },
+                u = this && this.__generator || function(t, e) {
+                    var r, n, i, o, u = {
+                        label: 0,
+                        sent: function() {
+                            if (1 & i[0]) throw i[1];
+                            return i[1]
+                        },
+                        trys: [],
+                        ops: []
+                    };
+                    return o = {
+                        next: s(0),
+                        throw: s(1),
+                        return: s(2)
+                    }, "function" == typeof Symbol && (o[Symbol.iterator] = function() {
+                        return this
+                    }), o;
 
-                function Nt(t, e, r) {
-                    if (void 0 === e) return t;
-                    switch (null == r ? 3 : r) {
-                        case 1:
-                            return function(r) {
-                                return t.call(e, r)
-                            };
-                        case 3:
-                            return function(r, n, i) {
-                                return t.call(e, r, n, i)
-                            };
-                        case 4:
-                            return function(r, n, i, o) {
-                                return t.call(e, r, n, i, o)
-                            }
-                    }
-                    return function() {
-                        return t.apply(e, arguments)
+                    function s(o) {
+                        return function(s) {
+                            return function(o) {
+                                if (r) throw new TypeError("Generator is already executing.");
+                                for (; u;) try {
+                                    if (r = 1, n && (i = 2 & o[0] ? n.return : o[0] ? n.throw || ((i = n.return) && i.call(n), 0) : n.next) && !(i = i.call(n, o[1])).done) return i;
+                                    switch (n = 0, i && (o = [2 & o[0], i.value]), o[0]) {
+                                        case 0:
+                                        case 1:
+                                            i = o;
+                                            break;
+                                        case 4:
+                                            return u.label++, {
+                                                value: o[1],
+                                                done: !1
+                                            };
+                                        case 5:
+                                            u.label++, n = o[1], o = [0];
+                                            continue;
+                                        case 7:
+                                            o = u.ops.pop(), u.trys.pop();
+                                            continue;
+                                        default:
+                                            if (!((i = (i = u.trys).length > 0 && i[i.length - 1]) || 6 !== o[0] && 2 !== o[0])) {
+                                                u = 0;
+                                                continue
+                                            }
+                                            if (3 === o[0] && (!i || o[1] > i[0] && o[1] < i[3])) {
+                                                u.label = o[1];
+                                                break
+                                            }
+                                            if (6 === o[0] && u.label < i[1]) {
+                                                u.label = i[1], i = o;
+                                                break
+                                            }
+                                            if (i && u.label < i[2]) {
+                                                u.label = i[2], u.ops.push(o);
+                                                break
+                                            }
+                                            i[2] && u.ops.pop(), u.trys.pop();
+                                            continue
+                                    }
+                                    o = e.call(t, u)
+                                } catch (t) {
+                                    o = [6, t], n = 0
+                                } finally {
+                                    r = i = 0
+                                }
+                                if (5 & o[0]) throw o[1];
+                                return {
+                                    value: o[0] ? o[1] : void 0,
+                                    done: !0
+                                }
+                            }([o, s])
+                        }
                     }
-                }
-
-                function $t(t, e, r) {
-                    return null == t ? Pt : $(t) ? Nt(t, e, r) : j(t) && !H(t) ? Mt(t) : zt(t)
-                }
-
-                function Rt(t, e) {
-                    return $t(t, e, 1 / 0)
-                }
-
-                function Bt(t, e, r) {
-                    return nt.iteratee !== Rt ? nt.iteratee(t, e) : $t(t, e, r)
-                }
-
-                function Ct() {}
-
-                function Ut(t, e) {
-                    return null == e && (e = t, t = 0), t + Math.floor(Math.random() * (e - t + 1))
-                }
-                nt.toPath = At, nt.iteratee = Rt;
-                var Ft = Date.now || function() {
-                    return (new Date).getTime()
                 };
-
-                function Ht(t) {
-                    var e = function(e) {
-                            return t[e]
-                        },
-                        r = "(?:" + et(t).join("|") + ")",
-                        n = RegExp(r),
-                        i = RegExp(r, "g");
-                    return function(t) {
-                        return t = null == t ? "" : "" + t, n.test(t) ? t.replace(i, e) : t
-                    }
-                }
-                var Dt = {
-                        "&": "&amp;",
-                        "<": "&lt;",
-                        ">": "&gt;",
-                        '"': "&quot;",
-                        "'": "&#x27;",
-                        "`": "&#x60;"
-                    },
-                    Lt = Ht(Dt),
-                    qt = Ht(mt(Dt)),
-                    Vt = nt.templateSettings = {
-                        evaluate: /<%([\s\S]+?)%>/g,
-                        interpolate: /<%=([\s\S]+?)%>/g,
-                        escape: /<%-([\s\S]+?)%>/g
-                    },
-                    Wt = /(.)^/,
-                    Jt = {
-                        "'": "'",
-                        "\\": "\\",
-                        "\r": "r",
-                        "\n": "n",
-                        "\u2028": "u2028",
-                        "\u2029": "u2029"
-                    },
-                    Gt = /\\|'|\r|\n|\u2028|\u2029/g;
-
-                function Kt(t) {
-                    return "\\" + Jt[t]
-                }
-                var Xt = /^\s*(\w|\$)+\s*$/,
-                    Qt = 0;
-
-                function Yt(t, e, r, n, i) {
-                    if (!(n instanceof e)) return t.apply(r, i);
-                    var o = Et(t.prototype),
-                        s = t.apply(o, i);
-                    return j(s) ? s : o
-                }
-                var Zt = x((function(t, e) {
-                    var r = Zt.placeholder,
-                        n = function() {
-                            for (var i = 0, o = e.length, s = Array(o), a = 0; a < o; a++) s[a] = e[a] === r ? arguments[i++] : e[a];
-                            for (; i < arguments.length;) s.push(arguments[i++]);
-                            return Yt(t, n, this, this, s)
-                        };
-                    return n
-                }));
-                Zt.placeholder = nt;
-                var te = x((function(t, e, r) {
-                        if (!$(t)) throw new TypeError("Bind must be called on a function");
-                        var n = x((function(i) {
-                            return Yt(t, n, e, this, r.concat(i))
-                        }));
-                        return n
-                    })),
-                    ee = J(Z);
-
-                function re(t, e, r, n) {
-                    if (n = n || [], e || 0 === e) {
-                        if (e <= 0) return n.concat(t)
-                    } else e = 1 / 0;
-                    for (var i = n.length, o = 0, s = Z(t); o < s; o++) {
-                        var a = t[o];
-                        if (ee(a) && (H(a) || q(a)))
-                            if (e > 1) re(a, e - 1, r, n), i = n.length;
-                            else
-                                for (var u = 0, c = a.length; u < c;) n[i++] = a[u++];
-                        else r || (n[i++] = a)
-                    }
-                    return n
-                }
-                var ne = x((function(t, e) {
-                        var r = (e = re(e, !1, !1)).length;
-                        if (r < 1) throw new Error("bindAll must be passed function names");
-                        for (; r--;) {
-                            var n = e[r];
-                            t[n] = te(t[n], t)
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            }), e.HubAsync = e.DEFAULT_CONFIG = void 0;
+            var s = r(80),
+                c = 1e3 / 3;
+            e.DEFAULT_CONFIG = {
+                METRIC_MODIFIER: 28.5,
+                TURN_MODIFIER: 2.56,
+                DRIVE_SPEED: 25,
+                TURN_SPEED: 20,
+                DEFAULT_STOP_DISTANCE: 105,
+                DEFAULT_CLEAR_DISTANCE: 120,
+                LEFT_MOTOR: "A",
+                RIGHT_MOTOR: "B",
+                VALID_MOTORS: ["A", "B"]
+            };
+            var a = function(t) {
+                    if (t.leftMotor = t.leftMotor || e.DEFAULT_CONFIG.LEFT_MOTOR, t.rightMotor = t.rightMotor || e.DEFAULT_CONFIG.RIGHT_MOTOR, !e.DEFAULT_CONFIG.VALID_MOTORS.includes(t.leftMotor)) throw Error("Define left port port correctly");
+                    if (!e.DEFAULT_CONFIG.VALID_MOTORS.includes(t.rightMotor)) throw Error("Define right port port correctly");
+                    if (t.leftMotor === t.rightMotor) throw Error("Left and right motor can not be same");
+                    t.distanceModifier = t.distanceModifier || e.DEFAULT_CONFIG.METRIC_MODIFIER, t.turnModifier = t.turnModifier || e.DEFAULT_CONFIG.TURN_MODIFIER, t.driveSpeed = t.driveSpeed || e.DEFAULT_CONFIG.DRIVE_SPEED, t.turnSpeed = t.turnSpeed || e.DEFAULT_CONFIG.TURN_SPEED, t.defaultStopDistance = t.defaultStopDistance || e.DEFAULT_CONFIG.DEFAULT_STOP_DISTANCE, t.defaultClearDistance = t.defaultClearDistance || e.DEFAULT_CONFIG.DEFAULT_CLEAR_DISTANCE
+                },
+                f = function(t, e, r) {
+                    var n = this;
+                    return void 0 === e && (e = function(t) {
+                        return n[t]
+                    }), void 0 === r && (r = 0), e.bind(this)(t) ? Promise.resolve(this[t]) : new Promise((function(i, s) {
+                        setTimeout((function() {
+                            return o(n, void 0, void 0, (function() {
+                                var n;
+                                return u(this, (function(o) {
+                                    switch (o.label) {
+                                        case 0:
+                                            return n = i, [4, f.bind(this)(t, e, r)];
+                                        case 1:
+                                            return [2, n.apply(void 0, [o.sent()])]
+                                    }
+                                }))
+                            }))
+                        }), r + 100)
+                    }))
+                },
+                h = function(t) {
+                    function e(e, r) {
+                        var n = t.call(this, e) || this;
+                        return a(r), n.configuration = r, n
+                    }
+                    return i(e, t), e.prototype.disconnectAsync = function() {
+                        return this.setDisconnected(), f.bind(this)("hubDisconnected")
+                    }, e.prototype.afterInitialization = function() {
+                        var t = this;
+                        this.hubDisconnected = null, this.portData = {
+                            A: {
+                                angle: 0
+                            },
+                            B: {
+                                angle: 0
+                            },
+                            AB: {
+                                angle: 0
+                            },
+                            C: {
+                                angle: 0
+                            },
+                            D: {
+                                angle: 0
+                            },
+                            LED: {
+                                angle: 0
+                            }
+                        }, this.useMetric = !0, this.modifier = 1, this.emitter.on("rotation", (function(e) {
+                            return t.portData[e.port].angle = e.angle
+                        })), this.emitter.on("disconnect", (function() {
+                            return t.hubDisconnected = !0
+                        })), this.emitter.on("distance", (function(e) {
+                            return t.distance = e
+                        }))
+                    }, e.prototype.ledAsync = function(t) {
+                        var e = this;
+                        return new Promise((function(r, n) {
+                            e.led(t, (function() {
+                                setTimeout(r, c)
+                            }))
+                        }))
+                    }, e.prototype.motorTimeAsync = function(t, e, r, n) {
+                        var i = this;
+                        return void 0 === r && (r = 100), void 0 === n && (n = !1), new Promise((function(o, u) {
+                            i.motorTime(t, e, r, (function() {
+                                setTimeout(o, n ? c + 1e3 * e : c)
+                            }))
+                        }))
+                    }, e.prototype.motorTimeMultiAsync = function(t, e, r, n) {
+                        var i = this;
+                        return void 0 === e && (e = 100), void 0 === r && (r = 100), void 0 === n && (n = !1), new Promise((function(o, u) {
+                            i.motorTimeMulti(t, e, r, (function() {
+                                setTimeout(o, n ? c + 1e3 * t : c)
+                            }))
+                        }))
+                    }, e.prototype.motorAngleAsync = function(t, e, r, n) {
+                        var i = this;
+                        return void 0 === r && (r = 100), void 0 === n && (n = !1), new Promise((function(s, a) {
+                            i.motorAngle(t, e, r, (function() {
+                                return o(i, void 0, void 0, (function() {
+                                    var e;
+                                    return u(this, (function(r) {
+                                        switch (r.label) {
+                                            case 0:
+                                                if (!n) return [3, 5];
+                                                e = void 0, r.label = 1;
+                                            case 1:
+                                                return e = this.portData[t].angle, [4, new Promise((function(t) {
+                                                    return setTimeout(t, c)
+                                                }))];
+                                            case 2:
+                                                r.sent(), r.label = 3;
+                                            case 3:
+                                                if (this.portData[t].angle !== e) return [3, 1];
+                                                r.label = 4;
+                                            case 4:
+                                                return s(), [3, 6];
+                                            case 5:
+                                                setTimeout(s, c), r.label = 6;
+                                            case 6:
+                                                return [2]
+                                        }
+                                    }))
+                                }))
+                            }))
+                        }))
+                    }, e.prototype.motorAngleMultiAsync = function(t, e, r, n) {
+                        var i = this;
+                        return void 0 === e && (e = 100), void 0 === r && (r = 100), void 0 === n && (n = !1), new Promise((function(s, a) {
+                            i.motorAngleMulti(t, e, r, (function() {
+                                return o(i, void 0, void 0, (function() {
+                                    var t;
+                                    return u(this, (function(e) {
+                                        switch (e.label) {
+                                            case 0:
+                                                if (!n) return [3, 5];
+                                                t = void 0, e.label = 1;
+                                            case 1:
+                                                return t = this.portData.AB.angle, [4, new Promise((function(t) {
+                                                    return setTimeout(t, c)
+                                                }))];
+                                            case 2:
+                                                e.sent(), e.label = 3;
+                                            case 3:
+                                                if (this.portData.AB.angle !== t) return [3, 1];
+                                                e.label = 4;
+                                            case 4:
+                                                return s(), [3, 6];
+                                            case 5:
+                                                setTimeout(s, c), e.label = 6;
+                                            case 6:
+                                                return [2]
+                                        }
+                                    }))
+                                }))
+                            }))
+                        }))
+                    }, e.prototype.useMetricUnits = function() {
+                        this.useMetric = !0
+                    }, e.prototype.useImperialUnits = function() {
+                        this.useMetric = !1
+                    }, e.prototype.setFrictionModifier = function(t) {
+                        this.modifier = t
+                    }, e.prototype.drive = function(t, e) {
+                        void 0 === e && (e = !0);
+                        var r = Math.abs(t) * ((this.useMetric ? this.configuration.distanceModifier : this.configuration.distanceModifier / 4) * this.modifier),
+                            n = this.configuration.driveSpeed * (t > 0 ? 1 : -1) * ("A" === this.configuration.leftMotor ? 1 : -1),
+                            i = this.configuration.driveSpeed * (t > 0 ? 1 : -1) * ("A" === this.configuration.leftMotor ? 1 : -1);
+                        return this.motorAngleMultiAsync(r, n, i, e)
+                    }, e.prototype.turn = function(t, e) {
+                        void 0 === e && (e = !0);
+                        var r = Math.abs(t) * this.configuration.turnModifier,
+                            n = "A" === this.configuration.leftMotor ? 1 : -1,
+                            i = this.configuration.turnSpeed * (t > 0 ? 1 : -1) * n,
+                            o = this.configuration.turnSpeed * (t > 0 ? -1 : 1) * n,
+                            u = "A" === this.configuration.leftMotor ? i : o,
+                            s = "A" === this.configuration.leftMotor ? o : i;
+                        return this.motorAngleMultiAsync(r, u, s, e)
+                    }, e.prototype.driveUntil = function(t, e) {
+                        return void 0 === t && (t = 0), void 0 === e && (e = !0), o(this, void 0, void 0, (function() {
+                            var r, n, i, o = this;
+                            return u(this, (function(u) {
+                                switch (u.label) {
+                                    case 0:
+                                        return r = 0 !== t ? this.useMetric ? t : 2.54 * t : this.configuration.defaultStopDistance, n = "A" === this.configuration.leftMotor ? 1 : -1, i = 1 === n ? function() {
+                                            return r >= o.distance
+                                        } : function() {
+                                            return r <= o.distance
+                                        }, this.motorTimeMulti(60, this.configuration.driveSpeed * n, this.configuration.driveSpeed * n), e ? [4, f.bind(this)("distance", i)] : [3, 3];
+                                    case 1:
+                                        return u.sent(), [4, this.motorAngleMultiAsync(0)];
+                                    case 2:
+                                        return u.sent(), [3, 4];
+                                    case 3:
+                                        return [2, f.bind(this)("distance", i).then((function(t) {
+                                            return o.motorAngleMulti(0, 0, 0)
+                                        }))];
+                                    case 4:
+                                        return [2]
+                                }
+                            }))
+                        }))
+                    }, e.prototype.turnUntil = function(t, e) {
+                        return void 0 === t && (t = 1), void 0 === e && (e = !0), o(this, void 0, void 0, (function() {
+                            var r, n = this;
+                            return u(this, (function(i) {
+                                switch (i.label) {
+                                    case 0:
+                                        return r = t > 0 ? 1 : -1, this.turn(360 * r, !1), e ? [4, f.bind(this)("distance", (function() {
+                                            return n.distance >= n.configuration.defaultClearDistance
+                                        }))] : [3, 3];
+                                    case 1:
+                                        return i.sent(), [4, this.turn(0, !1)];
+                                    case 2:
+                                        return i.sent(), [3, 4];
+                                    case 3:
+                                        return [2, f.bind(this)("distance", (function() {
+                                            return n.distance >= n.configuration.defaultClearDistance
+                                        })).then((function(t) {
+                                            return n.turn(0, !1)
+                                        }))];
+                                    case 4:
+                                        return [2]
+                                }
+                            }))
+                        }))
+                    }, e.prototype.updateConfiguration = function(t) {
+                        a(t), this.configuration = t
+                    }, e
+                }(s.Hub);
+            e.HubAsync = h
+        },
+        969: function(t, e, r) {
+            var n = this && this.__awaiter || function(t, e, r, n) {
+                    return new(r || (r = Promise))((function(i, o) {
+                        function u(t) {
+                            try {
+                                c(n.next(t))
+                            } catch (t) {
+                                o(t)
+                            }
                         }
-                        return t
-                    })),
-                    ie = x((function(t, e, r) {
-                        return setTimeout((function() {
-                            return t.apply(null, r)
-                        }), e)
-                    })),
-                    oe = Zt(ie, nt, 1);
-
-                function se(t) {
-                    return function() {
-                        return !t.apply(this, arguments)
-                    }
-                }
-
-                function ae(t, e) {
-                    var r;
-                    return function() {
-                        return --t > 0 && (r = e.apply(this, arguments)), t <= 1 && (e = null), r
-                    }
-                }
-                var ue = Zt(ae, 2);
-
-                function ce(t, e, r) {
-                    e = Bt(e, r);
-                    for (var n, i = et(t), o = 0, s = i.length; o < s; o++)
-                        if (e(t[n = i[o]], n, t)) return n
-                }
-
-                function le(t) {
-                    return function(e, r, n) {
-                        r = Bt(r, n);
-                        for (var i = Z(e), o = t > 0 ? 0 : i - 1; o >= 0 && o < i; o += t)
-                            if (r(e[o], o, e)) return o;
-                        return -1
-                    }
-                }
-                var he = le(1),
-                    fe = le(-1);
 
-                function pe(t, e, r, n) {
-                    for (var i = (r = Bt(r, n, 1))(e), o = 0, s = Z(t); o < s;) {
-                        var a = Math.floor((o + s) / 2);
-                        r(t[a]) < i ? o = a + 1 : s = a
-                    }
-                    return o
-                }
-
-                function de(t, e, r) {
-                    return function(n, i, o) {
-                        var s = 0,
-                            u = Z(n);
-                        if ("number" == typeof o) t > 0 ? s = o >= 0 ? o : Math.max(o + u, s) : u = o >= 0 ? Math.min(o + 1, u) : o + u + 1;
-                        else if (r && o && u) return n[o = r(n, i)] === i ? o : -1;
-                        if (i != i) return (o = e(a.call(n, s, u), V)) >= 0 ? o + s : -1;
-                        for (o = t > 0 ? s : u - 1; o >= 0 && o < u; o += t)
-                            if (n[o] === i) return o;
-                        return -1
-                    }
-                }
-                var ve = de(1, he, pe),
-                    ge = de(-1, fe);
-
-                function ye(t, e, r) {
-                    var n = (ee(t) ? he : ce)(t, e, r);
-                    if (void 0 !== n && -1 !== n) return t[n]
-                }
-
-                function _e(t, e, r) {
-                    var n, i;
-                    if (e = Nt(e, r), ee(t))
-                        for (n = 0, i = t.length; n < i; n++) e(t[n], n, t);
-                    else {
-                        var o = et(t);
-                        for (n = 0, i = o.length; n < i; n++) e(t[o[n]], o[n], t)
-                    }
-                    return t
-                }
-
-                function be(t, e, r) {
-                    e = Bt(e, r);
-                    for (var n = !ee(t) && et(t), i = (n || t).length, o = Array(i), s = 0; s < i; s++) {
-                        var a = n ? n[s] : s;
-                        o[s] = e(t[a], a, t)
-                    }
-                    return o
-                }
-
-                function me(t) {
-                    var e = function(e, r, n, i) {
-                        var o = !ee(e) && et(e),
-                            s = (o || e).length,
-                            a = t > 0 ? 0 : s - 1;
-                        for (i || (n = e[o ? o[a] : a], a += t); a >= 0 && a < s; a += t) {
-                            var u = o ? o[a] : a;
-                            n = r(n, e[u], u, e)
+                        function s(t) {
+                            try {
+                                c(n.throw(t))
+                            } catch (t) {
+                                o(t)
+                            }
                         }
-                        return n
-                    };
-                    return function(t, r, n, i) {
-                        var o = arguments.length >= 3;
-                        return e(t, Nt(r, i, 4), n, o)
-                    }
-                }
-                var xe = me(1),
-                    je = me(-1);
-
-                function we(t, e, r) {
-                    var n = [];
-                    return e = Bt(e, r), _e(t, (function(t, r, i) {
-                        e(t, r, i) && n.push(t)
-                    })), n
-                }
-
-                function Oe(t, e, r) {
-                    e = Bt(e, r);
-                    for (var n = !ee(t) && et(t), i = (n || t).length, o = 0; o < i; o++) {
-                        var s = n ? n[o] : o;
-                        if (!e(t[s], s, t)) return !1
-                    }
-                    return !0
-                }
 
-                function Se(t, e, r) {
-                    e = Bt(e, r);
-                    for (var n = !ee(t) && et(t), i = (n || t).length, o = 0; o < i; o++) {
-                        var s = n ? n[o] : o;
-                        if (e(t[s], s, t)) return !0
-                    }
-                    return !1
-                }
-
-                function Ee(t, e, r, n) {
-                    return ee(t) || (t = bt(t)), ("number" != typeof r || n) && (r = 0), ve(t, e, r) >= 0
-                }
-                var Ae = x((function(t, e, r) {
-                    var n, i;
-                    return $(e) ? i = e : (e = kt(e), n = e.slice(0, -1), e = e[e.length - 1]), be(t, (function(t) {
-                        var o = i;
-                        if (!o) {
-                            if (n && n.length && (t = It(t, n)), null == t) return;
-                            o = t[e]
+                        function c(t) {
+                            var e;
+                            t.done ? i(t.value) : (e = t.value, e instanceof r ? e : new r((function(t) {
+                                t(e)
+                            }))).then(u, s)
                         }
-                        return null == o ? o : o.apply(t, r)
+                        c((n = n.apply(t, e || [])).next())
                     }))
-                }));
-
-                function ke(t, e) {
-                    return be(t, zt(e))
-                }
-
-                function Ie(t, e, r) {
-                    var n, i, o = -1 / 0,
-                        s = -1 / 0;
-                    if (null == e || "number" == typeof e && "object" != typeof t[0] && null != t)
-                        for (var a = 0, u = (t = ee(t) ? t : bt(t)).length; a < u; a++) null != (n = t[a]) && n > o && (o = n);
-                    else e = Bt(e, r), _e(t, (function(t, r, n) {
-                        ((i = e(t, r, n)) > s || i === -1 / 0 && o === -1 / 0) && (o = t, s = i)
-                    }));
-                    return o
-                }
-                var Te = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
-
-                function Pe(t) {
-                    return t ? H(t) ? a.call(t) : E(t) ? t.match(Te) : ee(t) ? be(t, Pt) : bt(t) : []
-                }
-
-                function Me(t, e, r) {
-                    if (null == e || r) return ee(t) || (t = bt(t)), t[Ut(t.length - 1)];
-                    var n = Pe(t),
-                        i = Z(n);
-                    e = Math.max(Math.min(e, i), 0);
-                    for (var o = i - 1, s = 0; s < e; s++) {
-                        var a = Ut(s, o),
-                            u = n[s];
-                        n[s] = n[a], n[a] = u
-                    }
-                    return n.slice(0, e)
-                }
-
-                function ze(t, e) {
-                    return function(r, n, i) {
-                        var o = e ? [
-                            [],
-                            []
-                        ] : {};
-                        return n = Bt(n, i), _e(r, (function(e, i) {
-                            var s = n(e, i, r);
-                            t(o, e, s)
-                        })), o
-                    }
-                }
-                var Ne = ze((function(t, e, r) {
-                        D(t, r) ? t[r].push(e) : t[r] = [e]
-                    })),
-                    $e = ze((function(t, e, r) {
-                        t[r] = e
-                    })),
-                    Re = ze((function(t, e, r) {
-                        D(t, r) ? t[r]++ : t[r] = 1
-                    })),
-                    Be = ze((function(t, e, r) {
-                        t[r ? 0 : 1].push(e)
-                    }), !0);
-
-                function Ce(t, e, r) {
-                    return e in r
-                }
-                var Ue = x((function(t, e) {
-                        var r = {},
-                            n = e[0];
-                        if (null == t) return r;
-                        $(n) ? (e.length > 1 && (n = Nt(n, e[1])), e = at(t)) : (n = Ce, e = re(e, !1, !1), t = Object(t));
-                        for (var i = 0, o = e.length; i < o; i++) {
-                            var s = e[i],
-                                a = t[s];
-                            n(a, s, t) && (r[s] = a)
-                        }
-                        return r
-                    })),
-                    Fe = x((function(t, e) {
-                        var r, n = e[0];
-                        return $(n) ? (n = se(n), e.length > 1 && (r = e[1])) : (e = be(re(e, !1, !1), String), n = function(t, r) {
-                            return !Ee(e, r)
-                        }), Ue(t, n, r)
-                    }));
-
-                function He(t, e, r) {
-                    return a.call(t, 0, Math.max(0, t.length - (null == e || r ? 1 : e)))
-                }
-
-                function De(t, e, r) {
-                    return null == t || t.length < 1 ? null == e || r ? void 0 : [] : null == e || r ? t[0] : He(t, t.length - e)
-                }
-
-                function Le(t, e, r) {
-                    return a.call(t, null == e || r ? 1 : e)
-                }
-                var qe = x((function(t, e) {
-                        return e = re(e, !0, !0), we(t, (function(t) {
-                            return !Ee(e, t)
-                        }))
-                    })),
-                    Ve = x((function(t, e) {
-                        return qe(t, e)
-                    }));
-
-                function We(t, e, r, n) {
-                    O(e) || (n = r, r = e, e = !1), null != r && (r = Bt(r, n));
-                    for (var i = [], o = [], s = 0, a = Z(t); s < a; s++) {
-                        var u = t[s],
-                            c = r ? r(u, s, t) : u;
-                        e && !r ? (s && o === c || i.push(u), o = c) : r ? Ee(o, c) || (o.push(c), i.push(u)) : Ee(i, u) || i.push(u)
-                    }
-                    return i
-                }
-                var Je = x((function(t) {
-                    return We(re(t, !0, !0))
-                }));
-
-                function Ge(t) {
-                    for (var e = t && Ie(t, Z).length || 0, r = Array(e), n = 0; n < e; n++) r[n] = ke(t, n);
-                    return r
-                }
-                var Ke = x(Ge);
-
-                function Xe(t, e) {
-                    return t._chain ? nt(e).chain() : e
-                }
+                },
+                i = this && this.__generator || function(t, e) {
+                    var r, n, i, o, u = {
+                        label: 0,
+                        sent: function() {
+                            if (1 & i[0]) throw i[1];
+                            return i[1]
+                        },
+                        trys: [],
+                        ops: []
+                    };
+                    return o = {
+                        next: s(0),
+                        throw: s(1),
+                        return: s(2)
+                    }, "function" == typeof Symbol && (o[Symbol.iterator] = function() {
+                        return this
+                    }), o;
 
-                function Qe(t) {
-                    return _e(xt(t), (function(e) {
-                        var r = nt[e] = t[e];
-                        nt.prototype[e] = function() {
-                            var t = [this._wrapped];
-                            return s.apply(t, arguments), Xe(this, r.apply(nt, t))
-                        }
-                    })), nt
-                }
-                _e(["pop", "push", "reverse", "shift", "sort", "splice", "unshift"], (function(t) {
-                    var e = n[t];
-                    nt.prototype[t] = function() {
-                        var r = this._wrapped;
-                        return null != r && (e.apply(r, arguments), "shift" !== t && "splice" !== t || 0 !== r.length || delete r[0]), Xe(this, r)
-                    }
-                })), _e(["concat", "join", "slice"], (function(t) {
-                    var e = n[t];
-                    nt.prototype[t] = function() {
-                        var t = this._wrapped;
-                        return null != t && (t = e.apply(t, arguments)), Xe(this, t)
-                    }
-                }));
-                var Ye = Qe({
-                    __proto__: null,
-                    VERSION: t,
-                    restArguments: x,
-                    isObject: j,
-                    isNull: function(t) {
-                        return null === t
-                    },
-                    isUndefined: w,
-                    isBoolean: O,
-                    isElement: function(t) {
-                        return !(!t || 1 !== t.nodeType)
-                    },
-                    isString: E,
-                    isNumber: A,
-                    isDate: k,
-                    isRegExp: I,
-                    isError: T,
-                    isSymbol: P,
-                    isArrayBuffer: M,
-                    isDataView: F,
-                    isArray: H,
-                    isFunction: $,
-                    isArguments: q,
-                    isFinite: function(t) {
-                        return !P(t) && y(t) && !isNaN(parseFloat(t))
-                    },
-                    isNaN: V,
-                    isTypedArray: Y,
-                    isEmpty: function(t) {
-                        if (null == t) return !0;
-                        var e = Z(t);
-                        return "number" == typeof e && (H(t) || E(t) || q(t)) ? 0 === e : 0 === Z(et(t))
-                    },
-                    isMatch: rt,
-                    isEqual: function(t, e) {
-                        return st(t, e)
-                    },
-                    isMap: vt,
-                    isWeakMap: gt,
-                    isSet: yt,
-                    isWeakSet: _t,
-                    keys: et,
-                    allKeys: at,
-                    values: bt,
-                    pairs: function(t) {
-                        for (var e = et(t), r = e.length, n = Array(r), i = 0; i < r; i++) n[i] = [e[i], t[e[i]]];
-                        return n
-                    },
-                    invert: mt,
-                    functions: xt,
-                    methods: xt,
-                    extend: wt,
-                    extendOwn: Ot,
-                    assign: Ot,
-                    defaults: St,
-                    create: function(t, e) {
-                        var r = Et(t);
-                        return e && Ot(r, e), r
-                    },
-                    clone: function(t) {
-                        return j(t) ? H(t) ? t.slice() : wt({}, t) : t
-                    },
-                    tap: function(t, e) {
-                        return e(t), t
-                    },
-                    get: Tt,
-                    has: function(t, e) {
-                        for (var r = (e = kt(e)).length, n = 0; n < r; n++) {
-                            var i = e[n];
-                            if (!D(t, i)) return !1;
-                            t = t[i]
-                        }
-                        return !!r
-                    },
-                    mapObject: function(t, e, r) {
-                        e = Bt(e, r);
-                        for (var n = et(t), i = n.length, o = {}, s = 0; s < i; s++) {
-                            var a = n[s];
-                            o[a] = e(t[a], a, t)
-                        }
-                        return o
-                    },
-                    identity: Pt,
-                    constant: W,
-                    noop: Ct,
-                    toPath: At,
-                    property: zt,
-                    propertyOf: function(t) {
-                        return null == t ? Ct : function(e) {
-                            return Tt(t, e)
-                        }
-                    },
-                    matcher: Mt,
-                    matches: Mt,
-                    times: function(t, e, r) {
-                        var n = Array(Math.max(0, t));
-                        e = Nt(e, r, 1);
-                        for (var i = 0; i < t; i++) n[i] = e(i);
-                        return n
-                    },
-                    random: Ut,
-                    now: Ft,
-                    escape: Lt,
-                    unescape: qt,
-                    templateSettings: Vt,
-                    template: function(t, e, r) {
-                        !e && r && (e = r), e = St({}, e, nt.templateSettings);
-                        var n = RegExp([(e.escape || Wt).source, (e.interpolate || Wt).source, (e.evaluate || Wt).source].join("|") + "|$", "g"),
-                            i = 0,
-                            o = "__p+='";
-                        t.replace(n, (function(e, r, n, s, a) {
-                            return o += t.slice(i, a).replace(Gt, Kt), i = a + e.length, r ? o += "'+\n((__t=(" + r + "))==null?'':_.escape(__t))+\n'" : n ? o += "'+\n((__t=(" + n + "))==null?'':__t)+\n'" : s && (o += "';\n" + s + "\n__p+='"), e
-                        })), o += "';\n";
-                        var s, a = e.variable;
-                        if (a) {
-                            if (!Xt.test(a)) throw new Error("variable is not a bare identifier: " + a)
-                        } else o = "with(obj||{}){\n" + o + "}\n", a = "obj";
-                        o = "var __t,__p='',__j=Array.prototype.join,print=function(){__p+=__j.call(arguments,'');};\n" + o + "return __p;\n";
-                        try {
-                            s = new Function(a, "_", o)
-                        } catch (t) {
-                            throw t.source = o, t
-                        }
-                        var u = function(t) {
-                            return s.call(this, t, nt)
-                        };
-                        return u.source = "function(" + a + "){\n" + o + "}", u
-                    },
-                    result: function(t, e, r) {
-                        var n = (e = kt(e)).length;
-                        if (!n) return $(r) ? r.call(t) : r;
-                        for (var i = 0; i < n; i++) {
-                            var o = null == t ? void 0 : t[e[i]];
-                            void 0 === o && (o = r, i = n), t = $(o) ? o.call(t) : o
+                    function s(o) {
+                        return function(s) {
+                            return function(o) {
+                                if (r) throw new TypeError("Generator is already executing.");
+                                for (; u;) try {
+                                    if (r = 1, n && (i = 2 & o[0] ? n.return : o[0] ? n.throw || ((i = n.return) && i.call(n), 0) : n.next) && !(i = i.call(n, o[1])).done) return i;
+                                    switch (n = 0, i && (o = [2 & o[0], i.value]), o[0]) {
+                                        case 0:
+                                        case 1:
+                                            i = o;
+                                            break;
+                                        case 4:
+                                            return u.label++, {
+                                                value: o[1],
+                                                done: !1
+                                            };
+                                        case 5:
+                                            u.label++, n = o[1], o = [0];
+                                            continue;
+                                        case 7:
+                                            o = u.ops.pop(), u.trys.pop();
+                                            continue;
+                                        default:
+                                            if (!((i = (i = u.trys).length > 0 && i[i.length - 1]) || 6 !== o[0] && 2 !== o[0])) {
+                                                u = 0;
+                                                continue
+                                            }
+                                            if (3 === o[0] && (!i || o[1] > i[0] && o[1] < i[3])) {
+                                                u.label = o[1];
+                                                break
+                                            }
+                                            if (6 === o[0] && u.label < i[1]) {
+                                                u.label = i[1], i = o;
+                                                break
+                                            }
+                                            if (i && u.label < i[2]) {
+                                                u.label = i[2], u.ops.push(o);
+                                                break
+                                            }
+                                            i[2] && u.ops.pop(), u.trys.pop();
+                                            continue
+                                    }
+                                    o = e.call(t, u)
+                                } catch (t) {
+                                    o = [6, t], n = 0
+                                } finally {
+                                    r = i = 0
+                                }
+                                if (5 & o[0]) throw o[1];
+                                return {
+                                    value: o[0] ? o[1] : void 0,
+                                    done: !0
+                                }
+                            }([o, s])
                         }
-                        return t
-                    },
-                    uniqueId: function(t) {
-                        var e = ++Qt + "";
-                        return t ? t + e : e
-                    },
-                    chain: function(t) {
-                        var e = nt(t);
-                        return e._chain = !0, e
-                    },
-                    iteratee: Rt,
-                    partial: Zt,
-                    bind: te,
-                    bindAll: ne,
-                    memoize: function(t, e) {
-                        var r = function(n) {
-                            var i = r.cache,
-                                o = "" + (e ? e.apply(this, arguments) : n);
-                            return D(i, o) || (i[o] = t.apply(this, arguments)), i[o]
-                        };
-                        return r.cache = {}, r
-                    },
-                    delay: ie,
-                    defer: oe,
-                    throttle: function(t, e, r) {
-                        var n, i, o, s, a = 0;
-                        r || (r = {});
-                        var u = function() {
-                                a = !1 === r.leading ? 0 : Ft(), n = null, s = t.apply(i, o), n || (i = o = null)
+                    }
+                };
+            Object.defineProperty(e, "__esModule", {
+                value: !0
+            });
+            var o = r(990),
+                u = r(382),
+                s = r(14),
+                c = function() {
+                    function t() {
+                        this.logDebug = function(t) {}, this.deviceInfo = {
+                            ports: {
+                                A: {
+                                    action: "",
+                                    angle: 0
+                                },
+                                B: {
+                                    action: "",
+                                    angle: 0
+                                },
+                                AB: {
+                                    action: "",
+                                    angle: 0
+                                },
+                                C: {
+                                    action: "",
+                                    angle: 0
+                                },
+                                D: {
+                                    action: "",
+                                    angle: 0
+                                },
+                                LED: {
+                                    action: "",
+                                    angle: 0
+                                }
                             },
-                            c = function() {
-                                var c = Ft();
-                                a || !1 !== r.leading || (a = c);
-                                var l = e - (c - a);
-                                return i = this, o = arguments, l <= 0 || l > e ? (n && (clearTimeout(n), n = null), a = c, s = t.apply(i, o), n || (i = o = null)) : n || !1 === r.trailing || (n = setTimeout(u, l)), s
-                            };
-                        return c.cancel = function() {
-                            clearTimeout(n), a = 0, n = i = o = null
-                        }, c
-                    },
-                    debounce: function(t, e, r) {
-                        var n, i, o, s, a, u = function() {
-                                var c = Ft() - i;
-                                e > c ? n = setTimeout(u, e - c) : (n = null, r || (s = t.apply(a, o)), n || (o = a = null))
+                            tilt: {
+                                roll: 0,
+                                pitch: 0
                             },
-                            c = x((function(c) {
-                                return a = this, o = c, i = Ft(), n || (n = setTimeout(u, e), r && (s = t.apply(a, o))), s
-                            }));
-                        return c.cancel = function() {
-                            clearTimeout(n), n = o = a = null
-                        }, c
-                    },
-                    wrap: function(t, e) {
-                        return Zt(e, t)
-                    },
-                    negate: se,
-                    compose: function() {
-                        var t = arguments,
-                            e = t.length - 1;
-                        return function() {
-                            for (var r = e, n = t[e].apply(this, arguments); r--;) n = t[r].call(this, n);
-                            return n
-                        }
-                    },
-                    after: function(t, e) {
-                        return function() {
-                            if (--t < 1) return e.apply(this, arguments)
-                        }
-                    },
-                    before: ae,
-                    once: ue,
-                    findKey: ce,
-                    findIndex: he,
-                    findLastIndex: fe,
-                    sortedIndex: pe,
-                    indexOf: ve,
-                    lastIndexOf: ge,
-                    find: ye,
-                    detect: ye,
-                    findWhere: function(t, e) {
-                        return ye(t, Mt(e))
-                    },
-                    each: _e,
-                    forEach: _e,
-                    map: be,
-                    collect: be,
-                    reduce: xe,
-                    foldl: xe,
-                    inject: xe,
-                    reduceRight: je,
-                    foldr: je,
-                    filter: we,
-                    select: we,
-                    reject: function(t, e, r) {
-                        return we(t, se(Bt(e)), r)
-                    },
-                    every: Oe,
-                    all: Oe,
-                    some: Se,
-                    any: Se,
-                    contains: Ee,
-                    includes: Ee,
-                    include: Ee,
-                    invoke: Ae,
-                    pluck: ke,
-                    where: function(t, e) {
-                        return we(t, Mt(e))
-                    },
-                    max: Ie,
-                    min: function(t, e, r) {
-                        var n, i, o = 1 / 0,
-                            s = 1 / 0;
-                        if (null == e || "number" == typeof e && "object" != typeof t[0] && null != t)
-                            for (var a = 0, u = (t = ee(t) ? t : bt(t)).length; a < u; a++) null != (n = t[a]) && n < o && (o = n);
-                        else e = Bt(e, r), _e(t, (function(t, r, n) {
-                            ((i = e(t, r, n)) < s || i === 1 / 0 && o === 1 / 0) && (o = t, s = i)
-                        }));
-                        return o
-                    },
-                    shuffle: function(t) {
-                        return Me(t, 1 / 0)
-                    },
-                    sample: Me,
-                    sortBy: function(t, e, r) {
-                        var n = 0;
-                        return e = Bt(e, r), ke(be(t, (function(t, r, i) {
-                            return {
-                                value: t,
-                                index: n++,
-                                criteria: e(t, r, i)
-                            }
-                        })).sort((function(t, e) {
-                            var r = t.criteria,
-                                n = e.criteria;
-                            if (r !== n) {
-                                if (r > n || void 0 === r) return 1;
-                                if (r < n || void 0 === n) return -1
-                            }
-                            return t.index - e.index
-                        })), "value")
-                    },
-                    groupBy: Ne,
-                    indexBy: $e,
-                    countBy: Re,
-                    partition: Be,
-                    toArray: Pe,
-                    size: function(t) {
-                        return null == t ? 0 : ee(t) ? t.length : et(t).length
-                    },
-                    pick: Ue,
-                    omit: Fe,
-                    first: De,
-                    head: De,
-                    take: De,
-                    initial: He,
-                    last: function(t, e, r) {
-                        return null == t || t.length < 1 ? null == e || r ? void 0 : [] : null == e || r ? t[t.length - 1] : Le(t, Math.max(0, t.length - e))
-                    },
-                    rest: Le,
-                    tail: Le,
-                    drop: Le,
-                    compact: function(t) {
-                        return we(t, Boolean)
-                    },
-                    flatten: function(t, e) {
-                        return re(t, e, !1)
-                    },
-                    without: Ve,
-                    uniq: We,
-                    unique: We,
-                    union: Je,
-                    intersection: function(t) {
-                        for (var e = [], r = arguments.length, n = 0, i = Z(t); n < i; n++) {
-                            var o = t[n];
-                            if (!Ee(e, o)) {
-                                var s;
-                                for (s = 1; s < r && Ee(arguments[s], o); s++);
-                                s === r && e.push(o)
-                            }
-                        }
-                        return e
-                    },
-                    difference: qe,
-                    unzip: Ge,
-                    transpose: Ge,
-                    zip: Ke,
-                    object: function(t, e) {
-                        for (var r = {}, n = 0, i = Z(t); n < i; n++) e ? r[t[n]] = e[n] : r[t[n][0]] = t[n][1];
-                        return r
-                    },
-                    range: function(t, e, r) {
-                        null == e && (e = t || 0, t = 0), r || (r = e < t ? -1 : 1);
-                        for (var n = Math.max(Math.ceil((e - t) / r), 0), i = Array(n), o = 0; o < n; o++, t += r) i[o] = t;
-                        return i
-                    },
-                    chunk: function(t, e) {
-                        if (null == e || e < 1) return [];
-                        for (var r = [], n = 0, i = t.length; n < i;) r.push(a.call(t, n, n += e));
-                        return r
-                    },
-                    mixin: Qe,
-                    default: nt
-                });
-                return Ye._ = Ye, Ye
-            }()
+                            distance: Number.MAX_SAFE_INTEGER,
+                            rssi: 0,
+                            color: "",
+                            error: "",
+                            connected: !1
+                        }, this.controlData = {
+                            input: null,
+                            speed: 0,
+                            turnAngle: 0,
+                            tilt: {
+                                roll: 0,
+                                pitch: 0
+                            },
+                            forceState: null,
+                            updateInputMode: null,
+                            controlUpdateTime: void 0,
+                            state: void 0
+                        }
+                    }
+                    return t.prototype.connect = function(t) {
+                        return void 0 === t && (t = {}), n(this, void 0, void 0, (function() {
+                            var e, r;
+                            return i(this, (function(n) {
+                                switch (n.label) {
+                                    case 0:
+                                        return n.trys.push([0, 2, , 3]), this.configuration = t, [4, o.BoostConnector.connect(this.handleGattDisconnect.bind(this))];
+                                    case 1:
+                                        return e = n.sent(), this.initHub(e, this.configuration), [3, 3];
+                                    case 2:
+                                        return r = n.sent(), console.log("Error from connect: " + r), [3, 3];
+                                    case 3:
+                                        return [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.initHub = function(t, e) {
+                        return n(this, void 0, void 0, (function() {
+                            var r = this;
+                            return i(this, (function(o) {
+                                switch (o.label) {
+                                    case 0:
+                                        return this.hub = new u.HubAsync(t, e), this.hub.logDebug = this.logDebug, this.hub.emitter.on("disconnect", (function(t) {
+                                            return n(r, void 0, void 0, (function() {
+                                                return i(this, (function(t) {
+                                                    return [2]
+                                                }))
+                                            }))
+                                        })), this.hub.emitter.on("connect", (function(t) {
+                                            return n(r, void 0, void 0, (function() {
+                                                return i(this, (function(t) {
+                                                    switch (t.label) {
+                                                        case 0:
+                                                            return this.hub.afterInitialization(), [4, this.hub.ledAsync("white")];
+                                                        case 1:
+                                                            return t.sent(), this.logDebug("Connected"), [2]
+                                                    }
+                                                }))
+                                            }))
+                                        })), this.hubControl = new s.HubControl(this.deviceInfo, this.controlData, e), [4, this.hubControl.start(this.hub)];
+                                    case 1:
+                                        return o.sent(), this.updateTimer = setInterval((function() {
+                                            r.hubControl.update()
+                                        }), 100), [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.handleGattDisconnect = function() {
+                        return n(this, void 0, void 0, (function() {
+                            return i(this, (function(t) {
+                                return this.logDebug("handleGattDisconnect"), !1 === this.deviceInfo.connected || (this.hub.setDisconnected(), this.deviceInfo.connected = !1, clearInterval(this.updateTimer), this.logDebug("Disconnected")), [2]
+                            }))
+                        }))
+                    }, t.prototype.changeLed = function() {
+                        return n(this, void 0, void 0, (function() {
+                            return i(this, (function(t) {
+                                switch (t.label) {
+                                    case 0:
+                                        return this.hub && !1 !== this.hub.connected ? (this.color = "pink" === this.color ? "orange" : "pink", [4, this.hub.ledAsync(this.color)]) : [2];
+                                    case 1:
+                                        return t.sent(), [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.driveToDirection = function(t) {
+                        return void 0 === t && (t = 1), n(this, void 0, void 0, (function() {
+                            return i(this, (function(e) {
+                                switch (e.label) {
+                                    case 0:
+                                        return this.preCheck() ? t > 0 ? [4, this.hub.driveUntil()] : [3, 2] : [2];
+                                    case 1:
+                                    case 3:
+                                        return [2, e.sent()];
+                                    case 2:
+                                        return [4, this.hub.drive(-1e4)]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.disconnect = function() {
+                        if (this.hub && !1 !== this.hub.connected) return this.hub.setDisconnected(), o.BoostConnector.disconnect()
+                    }, t.prototype.ai = function() {
+                        this.hub && !1 !== this.hub.connected && this.hubControl.setNextState("Drive")
+                    }, t.prototype.stop = function() {
+                        return n(this, void 0, void 0, (function() {
+                            return i(this, (function(t) {
+                                switch (t.label) {
+                                    case 0:
+                                        return this.preCheck() ? (this.controlData.speed = 0, this.controlData.turnAngle = 0, [4, this.hub.motorTimeMultiAsync(1, 0, 0)]) : [2];
+                                    case 1:
+                                        return [2, t.sent()]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.updateConfiguration = function(t) {
+                        this.hub && (this.hub.updateConfiguration(t), this.hubControl.updateConfiguration(t))
+                    }, t.prototype.led = function(t) {
+                        this.preCheck() && this.hub.led(t)
+                    }, t.prototype.ledAsync = function(t) {
+                        return n(this, void 0, void 0, (function() {
+                            return i(this, (function(e) {
+                                switch (e.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.ledAsync(t)] : [2];
+                                    case 1:
+                                        return [2, e.sent()]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.motorTime = function(t, e, r) {
+                        void 0 === r && (r = 100), this.preCheck() && this.hub.motorTime(t, e, r)
+                    }, t.prototype.motorTimeAsync = function(t, e, r, o) {
+                        return void 0 === r && (r = 100), void 0 === o && (o = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(n) {
+                                switch (n.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.motorTimeAsync(t, e, r, o)] : [2];
+                                    case 1:
+                                        return n.sent(), [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.motorTimeMulti = function(t, e, r) {
+                        void 0 === e && (e = 100), void 0 === r && (r = 100), this.preCheck() && this.hub.motorTimeMulti(t, e, r)
+                    }, t.prototype.motorTimeMultiAsync = function(t, e, r, o) {
+                        return void 0 === e && (e = 100), void 0 === r && (r = 100), void 0 === o && (o = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(n) {
+                                switch (n.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.motorTimeMultiAsync(t, e, r, o)] : [2];
+                                    case 1:
+                                        return n.sent(), [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.motorAngle = function(t, e, r) {
+                        void 0 === r && (r = 100), this.preCheck() && this.hub.motorAngle(t, e, r)
+                    }, t.prototype.motorAngleAsync = function(t, e, r, o) {
+                        return void 0 === r && (r = 100), void 0 === o && (o = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(n) {
+                                switch (n.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.motorAngleAsync(t, e, r, o)] : [2];
+                                    case 1:
+                                        return n.sent(), [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.motorAngleMulti = function(t, e, r) {
+                        void 0 === e && (e = 100), void 0 === r && (r = 100), this.preCheck() && this.hub.motorAngleMulti(t, e, r)
+                    }, t.prototype.motorAngleMultiAsync = function(t, e, r, o) {
+                        return void 0 === e && (e = 100), void 0 === r && (r = 100), void 0 === o && (o = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(n) {
+                                switch (n.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.motorAngleMultiAsync(t, e, r, o)] : [2];
+                                    case 1:
+                                        return n.sent(), [2]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.drive = function(t, e) {
+                        return void 0 === e && (e = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(r) {
+                                switch (r.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.drive(t, e)] : [2];
+                                    case 1:
+                                        return [2, r.sent()]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.turn = function(t, e) {
+                        return void 0 === e && (e = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(r) {
+                                switch (r.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.turn(t, e)] : [2];
+                                    case 1:
+                                        return [2, r.sent()]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.driveUntil = function(t, e) {
+                        return void 0 === t && (t = 0), void 0 === e && (e = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(r) {
+                                switch (r.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.driveUntil(t, e)] : [2];
+                                    case 1:
+                                        return [2, r.sent()]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.turnUntil = function(t, e) {
+                        return void 0 === t && (t = 1), void 0 === e && (e = !0), n(this, void 0, void 0, (function() {
+                            return i(this, (function(r) {
+                                switch (r.label) {
+                                    case 0:
+                                        return this.preCheck() ? [4, this.hub.turnUntil(t, e)] : [2];
+                                    case 1:
+                                        return [2, r.sent()]
+                                }
+                            }))
+                        }))
+                    }, t.prototype.rawCommand = function(t) {
+                        if (this.preCheck()) return this.hub.rawCommand(t)
+                    }, t.prototype.preCheck = function() {
+                        return !(!this.hub || !1 === this.hub.connected || (this.hubControl.setNextState("Manual"), 0))
+                    }, t
+                }();
+            e.default = c
         }
     }
 ]);
```

### Comparing `ipylgbst-0.2.0/examples/lite/_output/extensions/bqplot/package.json` & `ipylgbst-0.2.1/ipylgbst/labextension/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5269362148268397%*

 * *Differences: {"'author'": "{'name': 'Thorsten Beier', 'email': 'derthorstenbeier@gmail.com'}",*

 * * "'bugs'": "OrderedDict([('url', 'https://github.com/jupyterlab-contrib-ipylgbst/issues')])",*

 * * "'dependencies'": "{'@jupyter-widgets/base': '^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6', "*

 * *                   "'@lumino/widgets': '^1.6.0', '@lumino/application': '^1.6.0', 'add': '^2.0.6', "*

 * *                   "'ieee754': '^1.2.1', 'lego-boost-browser': "*

 * *                   "'git+https://github.com/DerThorsten/lego-boost-browser.git',  […]*

```diff
@@ -1,111 +1,103 @@
 {
     "author": {
-        "email": "bqplot@bloomberg.net",
-        "name": "BQPlot Development team"
+        "email": "derthorstenbeier@gmail.com",
+        "name": "Thorsten Beier"
+    },
+    "bugs": {
+        "url": "https://github.com/jupyterlab-contrib-ipylgbst/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
-        "@lumino/messaging": "^1",
-        "@lumino/widgets": "^1",
-        "d3": "^5.7.0",
-        "d3-selection": "^1",
-        "is-typedarray": "^1.0.0",
-        "popper.js": "^1.0.0",
-        "three": "^0.91.0",
-        "topojson": "^1.6.24",
-        "underscore": "^1.8.3"
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6",
+        "@lumino/application": "^1.6.0",
+        "@lumino/widgets": "^1.6.0",
+        "add": "^2.0.6",
+        "ieee754": "^1.2.1",
+        "lego-boost-browser": "git+https://github.com/DerThorsten/lego-boost-browser.git"
     },
-    "description": "bqplot",
+    "description": "A widget library for controlling LEGO\u00ae BOOST via web-bluetooth",
     "devDependencies": {
-        "@jupyter-widgets/base-manager": "^1.0.0",
-        "@jupyter-widgets/controls": "^5",
+        "@babel/core": "^7.5.0",
+        "@babel/preset-env": "^7.5.0",
+        "@jupyter-widgets/base-manager": "^1.0.2",
         "@jupyterlab/builder": "^3.0.0",
-        "@types/chai": "^4.1.7",
-        "@types/d3": "^5.7.2",
-        "@types/expect.js": "^0.3.29",
-        "@types/mocha": "^7.0.2",
-        "@types/node": "^13.13.2",
-        "@types/sinon": "^9.0.0",
-        "chai": "^4.1.2",
-        "css-loader": "^5.0.0",
-        "eslint": "^7.22.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-config-standard": "^16.0.2",
-        "eslint-plugin-import": "^2.22.1",
-        "eslint-plugin-node": "^11.1.0",
-        "eslint-plugin-prettier": "^3.3.1",
-        "eslint-plugin-promise": "^4.2.1",
-        "karma": "^6.3.14",
-        "karma-chai": "^0.1.0",
-        "karma-chrome-launcher": "^3.1.0",
-        "karma-mocha": "^2.0.0",
-        "karma-mocha-reporter": "^2.2.5",
-        "karma-sinon": "^1.0.5",
-        "karma-sourcemap-loader": "^0.3.7",
-        "karma-typescript": "^5.0.2",
-        "karma-typescript-es6-transform": "^5.0.2",
-        "karma-webpack": "^5.0.0",
-        "less": "^3.8.1",
-        "less-loader": "^5.0.0",
-        "mocha": "^7.1.1",
+        "@types/jest": "^26.0.0",
+        "@types/webpack-env": "^1.13.6",
+        "@typescript-eslint/eslint-plugin": "^3.6.0",
+        "@typescript-eslint/parser": "^3.6.0",
+        "acorn": "^7.2.0",
+        "css-loader": "^3.2.0",
+        "eslint": "^7.4.0",
+        "eslint-config-prettier": "^6.11.0",
+        "eslint-plugin-prettier": "^3.1.4",
+        "fs-extra": "^7.0.0",
+        "identity-obj-proxy": "^3.0.0",
+        "jest": "^26.0.0",
+        "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
-        "prettier": "^2.2.1",
-        "raw-loader": "~4.0.1",
-        "rimraf": "^3.0.2",
-        "sinon": "^9.0.2",
-        "sinon-chai": "^3.3.0",
-        "style-loader": "^1.2.0",
-        "typescript": "^3.5.2",
-        "webpack": "^5",
-        "webpack-cli": "^3.3.12"
+        "prettier": "^2.0.5",
+        "rimraf": "^2.6.2",
+        "source-map-loader": "^1.1.3",
+        "style-loader": "^1.0.0",
+        "ts-jest": "^26.0.0",
+        "ts-loader": "^8.0.0",
+        "typescript": "~4.1.3",
+        "webpack": "^5.61.0",
+        "webpack-cli": "^4.0.0"
     },
     "files": [
-        "dist/",
-        "css/",
-        "lib/",
-        "shaders/"
+        "lib/**/*.js",
+        "dist/*.js",
+        "css/*.css"
     ],
+    "homepage": "https://github.com/jupyterlab-contrib-ipylgbst",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.99c828c2ee313756f7dc.js"
+            "load": "static/remoteEntry.b09d97918120529e3908.js"
         },
-        "extension": "lib/jupyterlab-plugin",
-        "outputDir": "../share/jupyter/labextensions/bqplot",
+        "extension": "lib/plugin",
+        "outputDir": "ipylgbst/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
-        },
-        "webpackConfig": "webpack.lab.config.js"
+        }
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
-        "jupyterlab notebook",
-        "jupyterlab-extension"
+        "jupyterlab-extension",
+        "widgets"
     ],
-    "license": "Apache-2.0",
+    "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "bqplot",
+    "name": "ipylgbst",
     "repository": {
         "type": "git",
-        "url": "https://github.com/bloomberg/bqplot.git"
+        "url": "https://github.com/jupyterlab-contrib-ipylgbst"
     },
     "scripts": {
-        "build": "jlpm run build:css && jlpm run build:js && jlpm run build:labextension && webpack --mode=production",
-        "build:css": "lessc less/bqplot.less css/bqplot.css",
-        "build:js": "tsc",
+        "build": "jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
-        "lint": "eslint . --ext .ts --fix",
-        "prepare": "jlpm run build",
-        "prettify": "yarn prettier --write .",
-        "test": "karma start --single-run",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc",
+        "build:nbextension": "webpack",
+        "build:prod": "jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension",
+        "clean": "jlpm run clean:lib && jlpm run clean:nbextension && jlpm run clean:labextension",
+        "clean:labextension": "rimraf ipylgbst/labextension",
+        "clean:lib": "rimraf lib",
+        "clean:nbextension": "rimraf ipylgbst/nbextension/static/index.js",
+        "install:extension": "jlpm build",
+        "lint": "eslint . --ext .ts,.tsx --fix",
+        "lint:check": "eslint . --ext .ts,.tsx",
+        "prepack": "jlpm run build:lib",
+        "test": "jest",
         "watch": "npm-run-all -p watch:*",
-        "watch:js": "tsc --watch",
         "watch:labextension": "jupyter labextension watch .",
+        "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
-    "version": "0.5.37"
+    "types": "./lib/index.d.ts",
+    "version": "0.2.1"
 }
```

### Comparing `ipylgbst-0.2.0/ipylgbst/__init__.py` & `ipylgbst-0.2.1/ipylgbst/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # Copyright (c) Thorsten Beier.
 # Distributed under the terms of the Modified BSD License.
 
 from .lego_boost import LegoBoostWidget, LedColor,Port, Sensor
-from ._version import __version__, version_info
+from ._version import __version__  # noqa
+
+version_info = __version__
 
 def _jupyter_labextension_paths():
     """Called by Jupyter Lab Server to detect if it is a valid labextension and
     to install the widget
     Returns
     =======
     src: Source directory name to copy files from. Webpack outputs generated files
```

### Comparing `ipylgbst-0.2.0/ipylgbst/tests/conftest.py` & `ipylgbst-0.2.1/ipylgbst/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/src/extension.ts` & `ipylgbst-0.2.1/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/src/plugin.ts` & `ipylgbst-0.2.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/src/version.ts` & `ipylgbst-0.2.1/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/src/widget.ts` & `ipylgbst-0.2.1/src/widget.ts`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,39 @@
 
 import { MODULE_NAME, MODULE_VERSION } from './version';
 
 // Import the CSS
 import '../css/widget.css';
 
 import LegoBoost from 'lego-boost-browser';
-const boost = new LegoBoost();
+
+// we use globals for the lego boost robot since connecting to
+// them takes a long time. If the model would hold the
+// boost instance, we would need to re-connect any time
+// we restart the kernel.
+
+interface deviceCache {
+  [key: string]: any;
+}
+
+const device_cache: deviceCache = {};
 
 export class LegoBoostModel extends DOMWidgetModel {
   defaults() {
     return {
       ...super.defaults(),
       _model_name: LegoBoostModel.model_name,
       _model_module: LegoBoostModel.model_module,
       _model_module_version: LegoBoostModel.model_module_version,
       _view_name: LegoBoostModel.view_name,
       _view_module: LegoBoostModel.view_module,
       _view_module_version: LegoBoostModel.view_module_version,
       _device_info: {},
+      name: 'device1',
+      n_lanes: 3,
     };
   }
 
   private save_device_info() {
     const device_info = {
       polling_frame: this.polling_frame,
       lane_cmd_index: this.lane_cmd_index,
@@ -51,24 +63,40 @@
     } else {
       this.polling_is_running = false;
     }
   }
 
   initialize(attributes: any, options: any) {
     super.initialize(attributes, options);
-    this.boost = boost; //new LegoBoost();
 
+    const n_lanes: number = this.get('n_lanes');
+    console.log(`initialize with n_lanes=${n_lanes}`, this);
+
+    const name: string = this.get('name');
+    console.log(`initialize with name=${name}`);
+    if (!(name in device_cache)) {
+      device_cache[name] = new LegoBoost();
+    }
+
+    this.boost = device_cache[name];
     this.on('msg:custom', async (command: any, buffers: any) => {
       const lane = command['lane'];
 
       this.lanes[lane] = this.lanes[lane].then(async () => {
-        await this.onCommand(command, buffers);
+        const await_in_kernel = <boolean>command['args'];
+        const await_in_frontend = <boolean>command['args'];
+        const p: Promise<void> = this.onCommand(command, buffers);
+        if (await_in_frontend) {
+          await p;
+        }
 
-        this.lane_cmd_index[lane] += 1;
-        this.save_device_info();
+        if (await_in_kernel) {
+          this.lane_cmd_index[lane] += 1;
+          this.save_device_info();
+        }
       });
     });
   }
 
   private async onCommand(command: any, buffers: any) {
     console.log('onCommand', command);
     const cmd = command['command'];
@@ -81,80 +109,68 @@
     } else {
       if (this.boost.deviceInfo.connected) {
         switch (cmd) {
           case 'poll':
             this.poll();
             break;
 
-          case 'drive':
-            await this.boost.drive.apply(this.boost, args);
-            break;
-
-          case 'turn':
-            await this.boost.turn.apply(this.boost, args);
+          case 'led':
+            this.boost.led.apply(this.boost, args);
             break;
-
-          case 'driveUntil':
-            await this.boost.driveUntil.apply(this.boost, args);
-            break;
-
-          case 'turnUntil':
-            await this.boost.turnUntil.apply(this.boost, args);
-            break;
-
           case 'ledAsync':
             await this.boost.ledAsync.apply(this.boost, args);
             break;
 
           case 'motorTime':
-            await this.boost.motorTime.apply(this.boost, args);
+            this.boost.motorTime.apply(this.boost, args);
             break;
 
           case 'motorTimeMulti':
-            await this.boost.motorTimeMulti.apply(this.boost, args);
+            this.boost.motorTimeMulti.apply(this.boost, args);
             break;
 
           case 'motorTimeAsync':
             await this.boost.motorTimeAsync.apply(this.boost, args);
             break;
 
           case 'motorTimeMultiAsync':
             await this.boost.motorTimeMultiAsync.apply(this.boost, args);
             break;
 
           case 'motorAngle':
-            await this.boost.motorAngle.apply(this.boost, args);
+            this.boost.motorAngle.apply(this.boost, args);
             break;
 
           case 'motorAngleMulti':
-            await this.boost.motorAngleMulti.apply(this.boost, args);
+            this.boost.motorAngleMulti.apply(this.boost, args);
             break;
 
           case 'motorAngleAsync':
             await this.boost.motorAngleAsync.apply(this.boost, args);
             break;
 
           case 'motorAngleMultiAsync':
             await this.boost.motorAngleMultiAsync.apply(this.boost, args);
             break;
 
           default:
-            console.log(`unknown command "${cmd}"`);
+            console.error(`unknown command "${cmd}"`);
             break;
         }
       } else {
         console.log(`cannot run command ${cmd} since we are not connected`);
       }
     }
   }
 
   async connect() {
     const sleep = (ms: number) => new Promise((r) => setTimeout(r, ms));
 
     if (!this.boost.deviceInfo.connected) {
+      console.log('not connected yet');
       await this.boost.connect();
 
       for (let i = 0; i < 30; i++) {
         await sleep(100);
         if (
           this.boost.deviceInfo.connected &&
           this.boost.hub !== undefined &&
@@ -162,14 +178,20 @@
         ) {
           break;
         }
       }
       await sleep(4000);
     }
 
+    // a bit ugly do this here
+    const n_lanes: number = this.get('n_lanes');
+    while (this.lane_cmd_index.length < n_lanes) {
+      this.lane_cmd_index.push(0);
+    }
+
     if (!this.polling_is_running) {
       this.polling_is_running = true;
       setTimeout(this.polling.bind(this), 200);
     }
   }
 
   static serializers: ISerializers = {
@@ -189,15 +211,15 @@
 
   private polling_frame = 0;
 
   private polling_is_running = false;
   stop_polling = false;
   //private currentProcessing: Promise<void> = Promise.resolve();
 
-  private lane_cmd_index: Array<number> = [0, 0, 0];
+  private lane_cmd_index: Array<number> = [0];
   private lanes: Array<Promise<void>> = [
     Promise.resolve(),
     Promise.resolve(),
     Promise.resolve(),
   ];
 
   static model_name = 'LegoBoostModel';
@@ -206,14 +228,15 @@
   static view_name = 'LegoBoostView'; // Set to null if no view
   static view_module = MODULE_NAME; // Set to null if no view
   static view_module_version = MODULE_VERSION;
 }
 
 export class LegoBoostView extends DOMWidgetView {
   txt_connected: HTMLDivElement;
+  txt_bluetooth: HTMLDivElement;
 
   txt_pitch: HTMLDivElement;
   txt_roll: HTMLDivElement;
   txt_distance: HTMLDivElement;
   txt_color: HTMLDivElement;
 
   txt_port_a: HTMLDivElement;
@@ -223,17 +246,36 @@
   txt_port_d: HTMLDivElement;
 
   meter_pitch: HTMLMeterElement;
   meter_roll: HTMLMeterElement;
   meter_distance: HTMLMeterElement;
   color_color: HTMLDivElement;
 
+  isWebBluetoothSupported: boolean = navigator.bluetooth ? true : false;
+
   render() {
     this.el.classList.add('custom-widget');
 
+    // checking if Web Bluetooth API is supported
+    if (!this.isWebBluetoothSupported) {
+      // bluetooth error box
+      const bluetooth_box = document.createElement('div');
+      bluetooth_box.classList.add('error-box');
+      this.el.appendChild(bluetooth_box);
+
+      this.txt_bluetooth = document.createElement('div');
+      this.txt_bluetooth.textContent =
+        "Your device doesn't support Web Bluetooth API. Try to turn on Experimental Platform Features from Chrome, by accessing the following link and turning it on: chrome://flags/#enable-experimental-web-platform-features";
+      bluetooth_box.appendChild(this.txt_bluetooth);
+
+      console.log(
+        "Your device doesn't support Web Bluetooth API. Try to turn on Experimental Platform Features from Chrome, by accessing the following link and turning it on: chrome://flags/#enable-experimental-web-platform-features"
+      );
+    }
+
     // connection box
     const connection_box = document.createElement('div');
     connection_box.classList.add('box');
     this.el.appendChild(connection_box);
 
     // sensor box
     const sensor_box = document.createElement('div');
```

### Comparing `ipylgbst-0.2.0/src/__tests__/index.spec.ts` & `ipylgbst-0.2.1/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/src/__tests__/utils.ts` & `ipylgbst-0.2.1/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/.gitignore` & `ipylgbst-0.2.1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
+# Version file is handled by hatchling
+ipylgbst/_version.py
+
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
 build/
```

### Comparing `ipylgbst-0.2.0/LICENSE.txt` & `ipylgbst-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipylgbst-0.2.0/README.md` & `ipylgbst-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 
 # ipylgbst
 
-[![Build Status](https://travis-ci.org/DerThorsten/ipylgbst.svg?branch=master)](https://travis-ci.org/DerThorsten/ipylgbst)
-[![codecov](https://codecov.io/gh/DerThorsten/ipylgbst/branch/master/graph/badge.svg)](https://codecov.io/gh/DerThorsten/ipylgbst)
+[![Github Actions Status](https://github.com/jupyterlab-contrib/ipylgbst/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/rise/actions/workflows/build.yml) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/ipylgbst/main)
 
+A widget library for controlling LEGO® BOOST via web-bluetooth.
 
-A widget library for controlling LEGO® BOOST via web-bluetooth
+https://user-images.githubusercontent.com/904752/223380492-a6b3dc34-064c-4b2c-a1d9-71f7712a8f57.mp4
 
 ## Installation
 
 You can install using `pip`:
 
 ```bash
 pip install ipylgbst
 ```
 
-If you are using Jupyter Notebook 5.2 or earlier, you may also need to enable
-the nbextension:
-```bash
-jupyter nbextension enable --py [--sys-prefix|--user|--system] ipylgbst
-```
-
 ## Development Installation
 
 Create a dev environment:
+
 ```bash
 conda create -n ipylgbst-dev -c conda-forge nodejs yarn python jupyterlab
 conda activate ipylgbst-dev
 ```
 
 Install the python. This will also build the TS package.
 ```bash
@@ -38,46 +33,41 @@
 notebook / lab frontend. For lab, this is done by the command:
 
 ```
 jupyter labextension develop --overwrite .
 yarn run build
 ```
 
-For classic notebook, you need to run:
-
-```
-jupyter nbextension install --sys-prefix --symlink --overwrite --py ipylgbst
-jupyter nbextension enable --sys-prefix --py ipylgbst
-```
-
 Note that the `--symlink` flag doesn't work on Windows, so you will here have to run
 the `install` command every time that you rebuild your extension. For certain installations
 you might also need another flag instead of `--sys-prefix`, but we won't cover the meaning
 of those flags here.
 
 ### How to see your changes
-#### Typescript:
+
+#### Typescript
+
 If you use JupyterLab to develop then you can watch the source directory and run JupyterLab at the same time in different
 terminals to watch for changes in the extension's source and automatically rebuild the widget.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
 yarn run watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 After a change wait for the build to finish and then refresh your browser and the changes should take effect.
 
-#### Python:
+#### Python
+
 If you make a change to the python code then you will need to restart the notebook kernel to have it take effect.
 
 ## Updating the version
 
 To update the version, install tbump and use it to bump the version.
 By default it will also create a tag.
 
 ```bash
 pip install tbump
 tbump <new-version>
 ```
-
```

### Comparing `ipylgbst-0.2.0/pyproject.toml` & `ipylgbst-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 [build-system]
-requires = [
-    "hatchling>=1.3.1",
-    "jupyterlab==3.*",
-]
+requires = ["hatchling>=1.4.0", "jupyterlab==3.*", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ipylgbst"
-description = "A widget library for controlling LEGO® BOOST via web-bluetooth"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.7"
-authors = [
-    { name = "Thorsten Beier", email = "derthorstenbeier@gmail.com" },
-]
-keywords = [
-    "IPython",
-    "Jupyter",
-    "Widgets",
-]
 classifiers = [
     "Framework :: Jupyter",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,15 +18,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
 ]
-version = "0.2.0"
+dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -50,16 +38,22 @@
 examples = []
 test = [
     "nbval",
     "pytest-cov",
     "pytest>=6.0",
 ]
 
-[project.urls]
-Homepage = "https://github.com/DerThorsten/ipylgbst"
+[tool.hatch.version]
+source = "nodejs"
+
+[tool.hatch.build.hooks.version]
+path = "ipylgbst/_version.py"
+
+[tool.hatch.metadata.hooks.nodejs]
+fields = ["description", "authors", "urls"]
 
 [tool.hatch.build]
 artifacts = [
     "ipylgbst/nbextension/index.*",
     "ipylgbst/labextension/*.tgz",
     "ipylgbst/labextension",
 ]
@@ -86,27 +80,25 @@
     "ipylgbst/labextension/package.json",
 ]
 dependencies = [
     "hatch-jupyter-builder>=0.5.0",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
-path = "."
 build_cmd = "build:prod"
+npm = ["jlpm"]
+
+[tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
+build_cmd = "install:extension"
+npm = ["jlpm"]
+source_dir = "src"
+build_dir = "ipylgbst/labextension"
+
+[tool.jupyter-releaser.options]
+version_cmd = "hatch version"
+
+[tool.jupyter-releaser.hooks]
+before-build-npm = ["python -m pip install jupyterlab~=3.0", "jlpm", "jlpm build:prod"]
+before-build-python = ["jlpm clean"]
 
-[tool.tbump]
-field = [
-    { name = "channel", default = "" },
-    { name = "release", default = "" },
-]
-file = [
-    { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
-    { src = "ipylgbst/_version.py" },
-]
-
-[tool.tbump.version]
-current = "0.1.3"
-regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
-
-[tool.tbump.git]
-message_template = "Bump to {new_version}"
-tag_template = "v{new_version}"
+[tool.check-wheel-contents]
+ignore = ["W002"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipylgbst-0.2.0/PKG-INFO` & `ipylgbst-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: ipylgbst
-Version: 0.2.0
+Version: 0.2.1
 Summary: A widget library for controlling LEGO® BOOST via web-bluetooth
-Project-URL: Homepage, https://github.com/DerThorsten/ipylgbst
+Project-URL: Homepage, https://github.com/jupyterlab-contrib-ipylgbst
+Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib-ipylgbst/issues
+Project-URL: Repository, https://github.com/jupyterlab-contrib-ipylgbst
 Author-email: Thorsten Beier <derthorstenbeier@gmail.com>
 License: Copyright (c) 2023 Thorsten Beier
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -28,15 +30,14 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE.txt
-Keywords: IPython,Jupyter,Widgets
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -60,37 +61,32 @@
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 
 # ipylgbst
 
-[![Build Status](https://travis-ci.org/DerThorsten/ipylgbst.svg?branch=master)](https://travis-ci.org/DerThorsten/ipylgbst)
-[![codecov](https://codecov.io/gh/DerThorsten/ipylgbst/branch/master/graph/badge.svg)](https://codecov.io/gh/DerThorsten/ipylgbst)
+[![Github Actions Status](https://github.com/jupyterlab-contrib/ipylgbst/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/rise/actions/workflows/build.yml) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/ipylgbst/main)
 
+A widget library for controlling LEGO® BOOST via web-bluetooth.
 
-A widget library for controlling LEGO® BOOST via web-bluetooth
+https://user-images.githubusercontent.com/904752/223380492-a6b3dc34-064c-4b2c-a1d9-71f7712a8f57.mp4
 
 ## Installation
 
 You can install using `pip`:
 
 ```bash
 pip install ipylgbst
 ```
 
-If you are using Jupyter Notebook 5.2 or earlier, you may also need to enable
-the nbextension:
-```bash
-jupyter nbextension enable --py [--sys-prefix|--user|--system] ipylgbst
-```
-
 ## Development Installation
 
 Create a dev environment:
+
 ```bash
 conda create -n ipylgbst-dev -c conda-forge nodejs yarn python jupyterlab
 conda activate ipylgbst-dev
 ```
 
 Install the python. This will also build the TS package.
 ```bash
@@ -101,46 +97,41 @@
 notebook / lab frontend. For lab, this is done by the command:
 
 ```
 jupyter labextension develop --overwrite .
 yarn run build
 ```
 
-For classic notebook, you need to run:
-
-```
-jupyter nbextension install --sys-prefix --symlink --overwrite --py ipylgbst
-jupyter nbextension enable --sys-prefix --py ipylgbst
-```
-
 Note that the `--symlink` flag doesn't work on Windows, so you will here have to run
 the `install` command every time that you rebuild your extension. For certain installations
 you might also need another flag instead of `--sys-prefix`, but we won't cover the meaning
 of those flags here.
 
 ### How to see your changes
-#### Typescript:
+
+#### Typescript
+
 If you use JupyterLab to develop then you can watch the source directory and run JupyterLab at the same time in different
 terminals to watch for changes in the extension's source and automatically rebuild the widget.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
 yarn run watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 After a change wait for the build to finish and then refresh your browser and the changes should take effect.
 
-#### Python:
+#### Python
+
 If you make a change to the python code then you will need to restart the notebook kernel to have it take effect.
 
 ## Updating the version
 
 To update the version, install tbump and use it to bump the version.
 By default it will also create a tag.
 
 ```bash
 pip install tbump
 tbump <new-version>
 ```
-
```

