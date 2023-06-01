# Comparing `tmp/pybdei-0.4.tar.gz` & `tmp/pybdei-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdei-0.4.tar", last modified: Tue May 16 10:58:11 2023, max compression
+gzip compressed data, was "pybdei-0.5.tar", last modified: Thu Jun  1 10:32:15 2023, max compression
```

## Comparing `pybdei-0.4.tar` & `pybdei-0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-16 10:58:11.925821 pybdei-0.4/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       59 2022-12-22 13:19:09.000000 pybdei-0.4/MANIFEST.in
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     5264 2023-05-16 10:58:11.925821 pybdei-0.4/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4625 2022-12-22 13:19:09.000000 pybdei-0.4/README.md
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-16 10:58:11.925821 pybdei-0.4/bdei/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    53789 2023-03-30 17:39:32.000000 pybdei-0.4/bdei/BDEI.cpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1053 2022-12-22 13:19:09.000000 pybdei-0.4/bdei/BDEI.hpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3718 2022-12-22 13:19:09.000000 pybdei-0.4/bdei/pool.hpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17217 2022-12-22 13:19:09.000000 pybdei-0.4/bdei/queue.hpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1745 2022-12-22 13:19:09.000000 pybdei-0.4/bdei/semaphore.hpp
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-16 10:58:11.925821 pybdei-0.4/pybdei/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     9566 2023-05-16 10:56:05.000000 pybdei-0.4/pybdei/__init__.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4609 2022-12-22 13:19:10.000000 pybdei-0.4/pybdei/_pybdei.cpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1205 2022-12-22 13:19:10.000000 pybdei-0.4/pybdei/_pybdei.hpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       84 2022-12-22 13:19:10.000000 pybdei-0.4/pybdei/_python.hpp
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6639 2022-12-22 13:19:10.000000 pybdei-0.4/pybdei/inference.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3962 2023-03-20 11:13:53.000000 pybdei-0.4/pybdei/loglikelihood.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-16 10:58:11.925821 pybdei-0.4/pybdei.egg-info/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     5264 2023-05-16 10:58:11.000000 pybdei-0.4/pybdei.egg-info/PKG-INFO
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      408 2023-05-16 10:58:11.000000 pybdei-0.4/pybdei.egg-info/SOURCES.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2023-05-16 10:58:11.000000 pybdei-0.4/pybdei.egg-info/dependency_links.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      100 2023-05-16 10:58:11.000000 pybdei-0.4/pybdei.egg-info/entry_points.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-05-16 10:58:11.000000 pybdei-0.4/pybdei.egg-info/requires.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-05-16 10:58:11.000000 pybdei-0.4/pybdei.egg-info/top_level.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-05-16 10:58:11.925821 pybdei-0.4/setup.cfg
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     2092 2023-05-16 10:56:05.000000 pybdei-0.4/setup.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-01 10:32:15.524289 pybdei-0.5/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       59 2022-12-22 13:19:09.000000 pybdei-0.5/MANIFEST.in
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     5264 2023-06-01 10:32:15.524289 pybdei-0.5/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4625 2022-12-22 13:19:09.000000 pybdei-0.5/README.md
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-01 10:32:15.524289 pybdei-0.5/bdei/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    54002 2023-06-01 10:30:25.000000 pybdei-0.5/bdei/BDEI.cpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1043 2023-06-01 10:30:25.000000 pybdei-0.5/bdei/BDEI.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3718 2022-12-22 13:19:09.000000 pybdei-0.5/bdei/pool.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17217 2022-12-22 13:19:09.000000 pybdei-0.5/bdei/queue.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1745 2022-12-22 13:19:09.000000 pybdei-0.5/bdei/semaphore.hpp
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-01 10:32:15.524289 pybdei-0.5/pybdei/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     8753 2023-06-01 10:30:25.000000 pybdei-0.5/pybdei/__init__.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4553 2023-06-01 10:30:25.000000 pybdei-0.5/pybdei/_pybdei.cpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1205 2022-12-22 13:19:10.000000 pybdei-0.5/pybdei/_pybdei.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       84 2022-12-22 13:19:10.000000 pybdei-0.5/pybdei/_python.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6062 2023-06-01 10:30:25.000000 pybdei-0.5/pybdei/inference.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3563 2023-06-01 10:30:25.000000 pybdei-0.5/pybdei/loglikelihood.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-01 10:32:15.524289 pybdei-0.5/pybdei.egg-info/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     5264 2023-06-01 10:32:15.000000 pybdei-0.5/pybdei.egg-info/PKG-INFO
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      408 2023-06-01 10:32:15.000000 pybdei-0.5/pybdei.egg-info/SOURCES.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2023-06-01 10:32:15.000000 pybdei-0.5/pybdei.egg-info/dependency_links.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      100 2023-06-01 10:32:15.000000 pybdei-0.5/pybdei.egg-info/entry_points.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-06-01 10:32:15.000000 pybdei-0.5/pybdei.egg-info/requires.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-06-01 10:32:15.000000 pybdei-0.5/pybdei.egg-info/top_level.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-06-01 10:32:15.524289 pybdei-0.5/setup.cfg
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     2092 2023-06-01 10:31:47.000000 pybdei-0.5/setup.py
```

### Comparing `pybdei-0.4/PKG-INFO` & `pybdei-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdei
-Version: 0.4
+Version: 0.5
 Summary: Fast and accurate epidemiological parameter estimation from phylogenetic trees with the Birth-Death Exposed-Infectious (BDEI) model.
 Home-page: https://github.com/evolbioinfo/BDEI
 Download-URL: https://github.com/evolbioinfo/BDEI
 Author: Frédéric Heicht
 Author-email: frederic.hecht@sorbonne-universite.fr
 Maintainer: Anna Zhukova
 Maintainer-email: anna.zhukova@pasteur.fr
```

### Comparing `pybdei-0.4/README.md` & `pybdei-0.5/README.md`

 * *Files identical despite different names*

### Comparing `pybdei-0.4/bdei/BDEI.cpp` & `pybdei-0.5/bdei/BDEI.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -832,23 +832,21 @@
 }
 
 int oneeee = 0;
 
 double duratinit = 0, duratopt = 0, duratbuild = 0, duraterr = 0;
 
 template<class RR>
-RR JCout(RR *x, R pie, R u, const vector<DataOde> &vdo, R eps = 1e-5) {
+RR JCout(RR *x, R pie, bool u, const vector<DataOde> &vdo, R eps = 1e-5) {
     RR Cout = 0;
     BDEI_pb<RR> pb(x, pie);
     int ni = 0;
     int n = (int) vdo.size();
     vector<RR> CC(n);
     assert(n);
-    R T = vdo[0].T;
-    assert(T);
     {
         thread_pool tp(size_pool);
         for (int i = 0; i < n; ++i) {
 
             RR *pCi = &CC[i];
             const DataOde *pvo = &vdo[i];
             if (pvo->internal()) ni++;
@@ -862,48 +860,57 @@
         Cout += CC[i];
     }
     //   exit(0);
     int fs = n - ni;
     int nt = ni + fs;//  nb de feuilles/ tips
     Cout += nt * log(pb.psi * pb.p); // sampling
     Cout += (nt - fs) * log(pb.la); // transmissions
-    Cout += u * log(pb.piE * pb.fU(T, 0) + pb.piI * pb.fU(T, 1)); // unsampled trees
+
+
+    if (u)
+    {
+        R T = vdo[0].T;
+        RR hidden_prob = pb.piE * pb.fU(T, 0) + pb.piI * pb.fU(T, 1);
+        RR u = RR(fs) / (RR(1.) - hidden_prob) * hidden_prob;
+//        cout << "Adding " << u << "hidden trees" << endl;
+        Cout += u * log(hidden_prob); // u unsampled trees
+    }
 
     return -Cout;
 }
 
 
 template<class RR>
-RR JCout(RR *x, R pie, R u, const vector<DataOde> &vdo, const vector<tuple<double, int, int >> &vs, R eps = 1e-5);
+RR JCout(RR *x, R pie, bool u, const vector<DataOde> &vdo, const vector<tuple<double, int, int >> &vs, R eps = 1e-5);
 
 class J_vdo {
 public:
     const vector<DataOde> &vdo;
     vector<tuple<double, int, int >> *vs;
     const R *p0;
-    R u;
+    bool u;
     R eps;
     R pie;
     long count;
     int debug;
     vector<int> num;
     int nn;
 
     double Jm;
     vector<double> xopt;
     double Jopt;//  value
     int dd, dsens;
     vector<double> dir; //
     int nnewton;
 
-    J_vdo(const vector<DataOde> &vdoo, const R *pp, R piee, R uu, R epss = 1e-6, int dd = 0)
+    J_vdo(const vector<DataOde> &vdoo, const R *pp, R piee, bool uu, R epss = 1e-6, int dd = 0)
             : vdo(vdoo), vs(0), p0(pp), pie(piee), u(uu), eps(epss), count(0), debug(dd), num(4), Jm(nan("")), xopt(), dd(0),
               dsens(0), dir(), nnewton(0) { init(); }
 
-    J_vdo(const vector<DataOde> &vdoo, vector<tuple<double, int, int >> &vss, const R *pp, R piee, R uu, R epss = 1e-6,
+    J_vdo(const vector<DataOde> &vdoo, vector<tuple<double, int, int >> &vss, const R *pp, R piee, bool uu, R epss = 1e-6,
           int dd = 0)
             : vdo(vdoo), vs(&vss), p0(pp), pie(piee), u(uu), eps(epss), count(0), debug(dd), num(4), Jm(nan("")), xopt(), dd(0),
               dsens(0), dir(4), nnewton(0) { init(); }
 
     void set(int ddd, int dds) {
         dd = ddd;
         dsens = dds;
@@ -912,15 +919,15 @@
     }
 
     void set(vector<double> &dd) { // direction ...
         dir = dd;
         assert(dd.size() == 4);
     }
 
-    J_vdo(const vector<DataOde> &vdoo, vector<tuple<double, int, int >> &vss, const R *pp, R piee, R uu, R epss, int dd,
+    J_vdo(const vector<DataOde> &vdoo, vector<tuple<double, int, int >> &vss, const R *pp, R piee, bool uu, R epss, int dd,
           double JJm, vector<double> xxopt, double JJopt)
             : vdo(vdoo), vs(&vss), p0(pp), pie(piee), u(uu), eps(epss), count(0),
               debug(dd), num(4), Jm(JJm), xopt(xxopt), Jopt(JJopt),
               dd(-1), dsens(-1), nnewton(0) { init(); }
 
     void init() {
         nn = 0;
@@ -1167,22 +1174,21 @@
 void mult(RR *m, RR *p) {
     RR x[] = {p[0], p[1]};
     p[0] = m[0] * x[0] + m[1] * x[1];
     p[1] = m[2] * x[0] + m[3] * x[1];
 }
 
 template<class RR>
-RR JCout(RR *x, R pie, R u, const vector<DataOde> &vdo, const vector<tuple<double, int, int >> &vs, R eps) {
+RR JCout(RR *x, R pie, bool u, const vector<DataOde> &vdo, const vector<tuple<double, int, int >> &vs, R eps) {
     RR Cout = 0;
     auto start = high_resolution_clock::now();
     BDEI_pb<RR> pb(x, pie);
     auto afterpb = high_resolution_clock::now();
     int ni = 0;// number of internal node ..
     int n = (int) vdo.size();
-    R T = vdo[0].T;
     vector<RR> m22 = Build(vs, pb, eps);
     auto afterbuild = high_resolution_clock::now();
     vector<RR> pp(4 * vdo.size());
     RR *pm22 = &m22[0];
     RR *ppp = &pp[0];
     RR pi[] = {pb.piE, pb.piI};
     RR *ppi = &pi[0];
@@ -1222,15 +1228,23 @@
     for (int i = 0; i < n; ++i)
         Cout += pp[i * 4];
 
     int fs = n - ni;
     int nt = ni + fs;//  nb de feuilles/ tips
     Cout += nt * log(pb.psi * pb.p); // sampling of tips
     Cout += (nt - fs) * log(pb.la); // transmissions
-    Cout += u * log(pb.piE * pb.fU(T, 0) + pb.piI * pb.fU(T, 1)); // unobserved trees
+
+    if (u)
+    {
+        R T = vdo[0].T;
+        RR hidden_prob = pb.piE * pb.fU(T, 0) + pb.piI * pb.fU(T, 1);
+        RR u = RR(fs) / (RR(1.) - hidden_prob) * hidden_prob;
+//        cout << "Adding " << u << "hidden trees" << endl;
+        Cout += u * log(hidden_prob); // u unsampled trees
+    }
     auto end = high_resolution_clock::now();
 
     duratinit += duration_cast<duration<double>>(afterpb - start).count();
     duratbuild += duration_cast<duration<double>>(afterbuild - afterpb).count();
     duratopt += duration_cast<duration<double>>(end - start).count();
 
     return -Cout;
@@ -1243,15 +1257,14 @@
     cout << "   -p       <value of p> \n";
     cout << "   -psi     <value of psi> \n";
     cout << "   -mu      <lock value of mu, (<0 unlock) > \n";
     cout << "   -p       <lock value of p, (<0 unlock)> \n";
     cout << "   -lambda  <lock value of lambda, , (<0 unlock)> \n";
     cout << "   -d       <value of debug> \n";
     cout << "   -T       <value of T> \n";
-    cout << "   -u       <value of u> \n";
     cout << "   -eps     <value of eps> \n";
     cout << "   -nt      <value of number of thread > \n";
     cout << "   -nbdirerr  <value> : nb of direction to compute error bound with random direction   \n";
     cout << "   -ferr    filename : to save bound err for graphic \n";
     cout << "   -err     compute optimal err bound   \n";
     cout << "   -old     previous algo \n";
     cout << "   -mma     mma optimizer \n";
@@ -1345,16 +1358,16 @@
 }
 
 vector<DataOde> &getForestDataODE(Forest &forest, R T, vector<DataOde> &vdo, int _debug) {
     if (T <= 0) {
         if (_debug >= infoVal)  cout << "Using tree-specific sampling periods (between tree start and tree's last sampled tip)." << endl;
         SetDataOde(forest, vdo);
     } else {
-        if (_debug >= infoVal)  cout << "Using global time " << T << " for the sampling period." << endl;
         T = max(T, forest.T);
+        if (_debug >= infoVal)  cout << "Using global time " << T << " for the sampling period." << endl;
         SetDataOde(forest, vdo, T);
     }
     return vdo;
 }
 
 
 vector<tuple<double, int, int>> &getVS(vector<DataOde> &vdo, vector<tuple<double, int, int>> &vs) {
@@ -1390,16 +1403,17 @@
         get<2>(vs[i]) = nk;
     }
     assert(nc == 0);
     return vs;
 }
 
 
-R calcLikelihood(Forest &forest, R mu, R lambda, R psi, R p, R pie, R T, R u, int _debug) {
+R calcLikelihood(Forest &forest, R mu, R lambda, R psi, R p, R pie, R T, int _debug) {
     vector<DataOde> vdo;
+    bool u = (T > 0) ? 1: 0;
     vdo = getForestDataODE(forest, T, vdo, _debug);
 
     vector<tuple<double, int, int >> vs;
     vs = getVS(vdo, vs);
 
     R predefdata[] = {mu, lambda, psi, p};
     double eps = 1e-6;
@@ -1419,23 +1433,23 @@
     opt.set_xtol_rel(1e-5);
     nlopt::result result = opt.optimize(xj, minf);
     return -minf;
 }
 
 
 
-R calculateLikelihood(const string &treename, R mu, R lambda, R psi, R p, R pie, R T, R u, int _debug) {
+R calculateLikelihood(const string &treename, R mu, R lambda, R psi, R p, R pie, R T, int _debug) {
     debug = _debug;
     Forest forest(treename);
-    return calcLikelihood(forest, mu, lambda, psi, p, pie, T, u, _debug);
+    return calcLikelihood(forest, mu, lambda, psi, p, pie, T, _debug);
 }
 
 
 Solution
-*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T, R u,
+*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T,
                 int nbdirerr, int nt, int debug_, int nStarts) {
     debug = debug_;
 
     Solution *s = nullptr;
     int num[4] = {0, 1, 2, 3}; // mu, la, psi , p
 
     double eps = 1e-6;
@@ -1450,26 +1464,27 @@
     rand_gen.seed(reng());
     algo = algo % 4;
     algo = min(3, max(0, algo));
 
 
     Forest forest(treename);
     vector<DataOde> vdo;
+    bool u = (T > 0) ? 1: 0;
     vdo = getForestDataODE(forest, T, vdo, debug_);
 
     vector<tuple<double, int, int >> vs;
     vs = getVS(vdo, vs);
 
     R cpu_time = 0.00;
     int nb_iter = 0;
 
     if (debug >= debugVal)
         cout << "forest file: " << treename << endl;
 //             << ", mu  = " << mu << ", lambda = " << lambda << ", psi = " << psi << ", p = " << p
-//             << ", T = " << T << ", u = " << u << endl;
+//             << ", T = " << T << endl;
     R predefdata[] = {mu, lambda, psi, p};
     vector<double> xsol(4); // to store the solution ...
     int nbdata = 0;
 
     for (int k = 0; k < 4; ++k)
         if (predefdata[k] < 0) {
             num[nbdata++] = k;
@@ -1506,16 +1521,16 @@
         }
         if (debug >= infoVal)
         {
             cout << "Optimisation attempt " << startI + 1 << ":" << endl;
             cout << "  starting values for optimised parameters: " << xj << endl;
             cout << "  upper bounds : " << ub << endl;
 
-            R sol2 = calcLikelihood(forest, xj[0], xj[1], xj[2], x0[3], pie, T, u, 0);
-            cout << "  initial log-likelihood: " << setprecision(10) << sol2 << endl;
+//            R sol2 = calcLikelihood(forest, xj[0], xj[1], xj[2], x0[3], pie, T, 0);
+//            cout << "  initial log-likelihood: " << setprecision(10) << sol2 << endl;
         }
         bool ok = false;
         try {
             nlopt::result result = opt.optimize(xj, minf);
             ok = true;
             if (debug >= infoVal)
             {
@@ -1565,28 +1580,28 @@
         s = new Solution(-Jsol, sol[0], sol[1], sol[2], sol[3], cpu_time, nb_iter);
     }
     return s;
 }
 
 
 Solution
-*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T, R u,
+*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T,
                 int nbdirerr, int nt, int nstarts) {
-    return inferParameters(treename, x0, dub, pie, mu, lambda, psi, p, T, u, nbdirerr, nt, infoVal, nstarts);
+    return inferParameters(treename, x0, dub, pie, mu, lambda, psi, p, T, nbdirerr, nt, infoVal, nstarts);
 }
 
 Solution
-*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T, R u, int nbdirerr, int nt) {
-    return inferParameters(treename, x0, dub, pie, mu, lambda, psi, p, T, u, nbdirerr, nt, infoVal, 1);
+*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T, int nbdirerr, int nt) {
+    return inferParameters(treename, x0, dub, pie, mu, lambda, psi, p, T, nbdirerr, nt, infoVal, 1);
 }
 
 int main(int argc, const char *argv[]) {
     string treename = "";
     int nbdirerr = 0;
-    R T = 0, u = 0;
+    R T = 0;
     R p = -1;
     R mu = -1;
     R lambda = -1;
     R psi = -1;
     int kk = 0;
 
     R x0[] = {0.5, .1, 0.6, 0.8}; // default starting points
@@ -1623,18 +1638,14 @@
             lambda = atof(argv[kk + 2]);
             kk += 2;
         }
         else if (argc > kk + 2 && strcmp(argv[kk + 1], "-T") == 0) {
             T = atof(argv[kk + 2]);
             kk += 2;
         }
-        else if (argc > kk + 2 && strcmp(argv[kk + 1], "-u") == 0) {
-            u = atof(argv[kk + 2]);
-            kk += 2;
-        }
         else if (argc > kk + 2 && strcmp(argv[kk + 1], "-nt") == 0) {
             size_pool = atoi(argv[kk + 2]);
             kk += 2;
         }
         else if (argc > kk + 2 && strcmp(argv[kk + 1], "-d") == 0) {
             debug = atof(argv[kk + 2]);
             kk += 2;
@@ -1657,13 +1668,13 @@
             showparam(x0, treename, algo_name);
             return 1;
         }
 
     }
     if (argc > ++kk) treename = argv[kk];
 
-    Solution *res = inferParameters(treename, x0, dub, -1., mu, lambda, psi, p, T, u, nbdirerr, size_pool, debug, 1);
+    Solution *res = inferParameters(treename, x0, dub, -1., mu, lambda, psi, p, T, nbdirerr, size_pool, debug, 1);
     if (res) {
         return 0;
     }
     return -1;
 }
```

### Comparing `pybdei-0.4/bdei/BDEI.hpp` & `pybdei-0.5/bdei/BDEI.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -32,10 +32,10 @@
 
     Solution(R l, R mu_, R la_, R psi_, R p_, R cpu_time_, int nb_iter_);
     Solution(R l, R mu_, R mu_min_, R mu_max_, R la_, R la_min_, R la_max_, R psi_, R psi_min_, R psi_max_, R p_, R p_min_, R p_max_, R cpu_time_, int nb_iter_);
 };
 
 
 Solution
-*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T, R u, int nbdirerr, int size_pool, int debug_, int nstarts);
+*inferParameters(const string &treename, R *x0, const R *dub, R pie, R mu, R lambda, R psi, R p, R T, int nbdirerr, int size_pool, int debug_, int nstarts);
 
-R calculateLikelihood(const string &treename, R mu, R lambda, R psi, R p, R pie, R T, R u, int debug_);
+R calculateLikelihood(const string &treename, R mu, R lambda, R psi, R p, R pie, R T, int debug_);
```

### Comparing `pybdei-0.4/bdei/pool.hpp` & `pybdei-0.5/bdei/pool.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.4/bdei/queue.hpp` & `pybdei-0.5/bdei/queue.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.4/bdei/semaphore.hpp` & `pybdei-0.5/bdei/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.4/pybdei/__init__.py` & `pybdei-0.5/pybdei/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,249 +1,238 @@
-import os
-from collections import namedtuple
-
-import _pybdei
-import numpy as np
-from ete3 import Tree
-
-ERRORS = 0
-WARNINGS = 1
-INFO = 2
-DEBUG = 3
-
-PYBDEI_VERSION = 0.4
-
-PS = (0.1, 0.4, 0.7)
-
-BDEI_result = namedtuple('BDEI_result', ['mu', 'la', 'psi', 'p', 'mu_CI', 'la_CI', 'psi_CI', 'p_CI',
-                                         'R_naught', 'incubation_period', 'infectious_time'])
-BDEI_time = namedtuple('BDEI_time', ['CPU_time', 'iterations'])
-
-
-def parse_tree(nwk):
-    """Parses an input tree in newick format and checks if it is binary and rooted"""
-    tree = None
-    for f in (0, 1, 2, 3, 5):
-        try:
-            tree = Tree(nwk, format=f)
-            break
-        except:
-            pass
-    if not tree:
-        raise ValueError("Please make sure to use correct newick format and to specify branch lengths.")
-    if len(tree.children) > 2:
-        raise ValueError("The input tree must be rooted and binary, please root your tree.")
-    for _ in tree.traverse():
-        n_children = len(_.children)
-        if not _.is_leaf() and n_children != 2:
-            raise ValueError("The input tree must be binary, while your tree contains internal nodes with {} children, "
-                             "please fix it.".format(n_children))
-        if not _.is_root() and _.dist == 0:
-            raise ValueError("The input tree must not contain non-root zero branches, while your tree does, "
-                             "please fix it.")
-    return tree
-
-
-def parse_forest(nwk):
-    res = []
-    with open(nwk, 'r') as f:
-        res = [parse_tree(_.strip('\n') + ';') for _ in f.read().split(';')[:-1]]
-    if not res:
-        raise ValueError('Could not find any trees in your input file (check the newick format): {}'.format(nwk))
-    return res
-
-
-def save_tree(tree, nwk):
-    with open(nwk, 'w+') as f:
-        f.write('{}\n'.format(tree.write(format=5, format_root_node=True)))
-
-
-def save_forest(forest, nwk):
-    with open(nwk, 'w+') as f:
-        for tree in forest:
-            _ = tree.write(format=5, format_root_node=True)
-            f.write('{}\n'.format(_))
-
-
-def initial_rate_guess(forest, mu=None, la=None, psi=None):
-
-    fixed_rates = []
-    for rate in (mu, la, psi):
-        if rate and rate > 0:
-            fixed_rates.append(rate)
-    if fixed_rates:
-        avg_rate = np.average(fixed_rates)
-        min_rate = avg_rate
-        max_rate = avg_rate
-    else:
-        internal_is, external_is = [], []
-        internal_es, external_es = [], []
-        for tree in forest:
-            for n in tree.traverse('preorder'):
-                if not n.is_leaf():
-                    i, e = sorted(n.children, key=lambda c: c.dist)
-                    (internal_is if not i.is_leaf() else external_is).append(i)
-                    (internal_es if not i.is_leaf() else external_es).append(e)
-        i_s_times = np.array([_.dist for _ in external_is])
-        i_tr_times = np.array([_.dist for _ in internal_is])
-        e_s_times = np.array([_.dist for _ in external_es])
-        e_tr_times = np.array([_.dist for _ in internal_es])
-        i_s_time = np.median(i_s_times)
-        e_s_time = np.median(e_s_times)
-        # if it is a corner case when we only have tips, let's use sampling times
-        i_tr_time = np.median(i_tr_times) if len(i_tr_times) else i_s_time
-        e_tr_time = np.median(e_tr_times) if len(e_tr_times) else e_s_time
-        mu_times = []
-        if e_s_time > i_s_time:
-            mu_times.append(e_s_time - i_s_time)
-        if e_tr_time > i_tr_time:
-            mu_times.append(e_tr_time - i_tr_time)
-        mu_time = np.average(mu_times) if mu_times else min(i_s_time, i_tr_time) * 0.01
-        avg_rate = np.average([1 / i_s_time, 1 / i_tr_time, 1 / mu_time])
-        min_rate = min([1 / i_s_time, 1 / i_tr_time, 1 / mu_time])
-        max_rate = max([1 / i_s_time, 1 / i_tr_time, 1 / mu_time])
-
-    return sorted({avg_rate, min_rate, max_rate})
-
-
-def infer(nwk, start=None, upper_bounds=None, pi_E=-1,
-          mu=-1, la=-1, psi=-1, p=-1, T=0.0, u=0, CI_repetitions=0, threads=1, log_level=INFO, **kwargs):
-    """Infer BDEI parameters from a phylogenetic tree."""
-
-    forest = None
-
-    if u > 0 and T <= 0:
-        raise ValueError("The number of unobserved trees is positive (u={}), "
-                         "hence all the trees are assumed to have started at the same time, "
-                         "and a non-zero T must be given.".format(u))
-
-    if isinstance(start, BDEI_result):
-        start = np.array([start.mu, start.la, start.psi, start.p])
-    if start is None:
-        forest = parse_forest(nwk)
-        if not p or p <= 0 or p >= 1:
-            rate = initial_rate_guess(forest, mu, la, psi).pop()
-            starts = [[rate, rate, rate, pp] for pp in PS]
-        else:
-            starts = [[rate, rate, rate, p] for rate in initial_rate_guess(forest, mu, la, psi)]
-    else:
-        starts = [start]
-    for s in starts:
-        s[-1] = min(0.99, max(0.001, s[-1]))
-
-    if upper_bounds is None:
-        upper_bounds = np.array([np.inf, np.inf, np.inf, 1])
-    elif isinstance(upper_bounds, BDEI_result):
-        upper_bounds = np.array([upper_bounds.mu, upper_bounds.la, upper_bounds.psi, upper_bounds.p])
-    else:
-        upper_bounds = np.array(upper_bounds)
-    if any(upper_bounds <= 0):
-        raise ValueError('Upper bound must be positive.')
-    upper_bounds[-1] = min(upper_bounds[-1], 1)
-
-    if pi_E is not None and pi_E >= 0:
-        if pi_E > 1:
-            raise ValueError('Frequencies of pi_E should be between 0 and 1.')
-    else:
-        pi_E = -1
-
-    something_is_fixed = False
-    all_is_fixed = True
-    if mu >= 0:
-        upper_bounds[0] = mu
-        for s in starts:
-            s[0] = mu
-        something_is_fixed = True
-    else:
-        all_is_fixed = False
-    if la >= 0:
-        upper_bounds[1] = la
-        for s in starts:
-            s[1] = la
-        something_is_fixed = True
-    else:
-        all_is_fixed = False
-    if psi >= 0:
-        upper_bounds[2] = psi
-        for s in starts:
-            s[2] = psi
-        something_is_fixed = True
-    else:
-        all_is_fixed = False
-    if 0 < p <= 1:
-        upper_bounds[3] = p
-        for s in starts:
-            s[3] = p
-        something_is_fixed = True
-    else:
-        all_is_fixed = False
-
-    if not something_is_fixed:
-        raise ValueError('To be identifiable, the BDEI model needs one of its parameters to be fixed. '
-                         'Please do so, using one of the following arguments: mu, la, psi, p.')
-    if all_is_fixed:
-        raise ValueError('At least one of the following arguments: mu, la, psi, p, should be left to be optimised.')
-    starts = [np.minimum(s, upper_bounds * 0.999) for s in starts]
-    nstarts = len(starts)
-    starts = np.reshape(starts, (4 * nstarts,))
-
-    def get_res(_nwk):
-        return _pybdei.infer(f=_nwk, start=starts, ub=upper_bounds, pie=pi_E,
-                             mu=mu, la=la, psi=psi, p=p, T=T, u=u, nt=threads, nbiter=CI_repetitions,
-                             debug=log_level, nstarts=nstarts)
-
-    try:
-        res = get_res(nwk)
-    except:
-        temp_nwk = nwk + '.temp'
-        if forest is None:
-            forest = parse_forest(nwk)
-        save_forest(forest, temp_nwk)
-        res = get_res(temp_nwk)
-        try:
-            os.remove(temp_nwk)
-        except OSError:
-            pass
-
-    return BDEI_result(mu=res[0], la=res[1], psi=res[2], p=res[3],
-                       mu_CI=(res[4], res[5]) if CI_repetitions > 0 else None,
-                       la_CI=(res[6], res[7]) if CI_repetitions > 0 else None,
-                       psi_CI=(res[8], res[9]) if CI_repetitions > 0 else None,
-                       p_CI=(res[10], res[11]) if CI_repetitions > 0 else None,
-                       R_naught=res[1] / res[2], incubation_period=1 / res[0], infectious_time=1 / res[2]), \
-           BDEI_time(CPU_time=res[13], iterations=res[14])
-
-
-def get_loglikelihood(nwk, mu=-1, la=-1, psi=-1, p=-1, pi_E=-1, T=0.0, u=0, log_level=INFO, params=None, **kwargs):
-    """Calculate loglikelihood for given BDEI parameters from a phylogenetic tree."""
-
-    if u > 0 and T <= 0:
-        raise ValueError("The number of unobserved trees is positive (u={}), "
-                         "hence all the trees are assumed to have started at the same time, "
-                         "and a non-zero T must be given.".format(u))
-
-    if params is not None:
-        if isinstance(params, BDEI_result):
-            mu = params.mu
-            la = params.la
-            psi = params.psi
-            p = params.p
-        else:
-            [mu, la, psi, p] = params
-    for par in [mu, la, psi, p]:
-        if par is None or par < 0:
-            raise ValueError('All the parameters (mu, la, psi, p) must be specified, '
-                             'either via dedicated arguments or via the params argument')
-
-    try:
-        res = _pybdei.likelihood(f=nwk, mu=mu, la=la, psi=psi, p=p, pie=pi_E, T=T, u=u, debug=log_level)
-    except:
-        temp_nwk = nwk + '.temp'
-        forest = parse_forest(nwk)
-        save_forest(forest, temp_nwk)
-        res = _pybdei.likelihood(f=temp_nwk, mu=mu, la=la, psi=psi, p=p, pie=pi_E, T=T, u=u, debug=log_level)
-        try:
-            os.remove(temp_nwk)
-        except OSError:
-            pass
-    return res
-
+import os
+from collections import namedtuple
+
+import _pybdei
+import numpy as np
+from ete3 import Tree
+
+ERRORS = 0
+WARNINGS = 1
+INFO = 2
+DEBUG = 3
+
+PYBDEI_VERSION = 0.4
+
+PS = (0.1, 0.4, 0.7)
+
+BDEI_result = namedtuple('BDEI_result', ['mu', 'la', 'psi', 'p', 'mu_CI', 'la_CI', 'psi_CI', 'p_CI',
+                                         'R_naught', 'incubation_period', 'infectious_time'])
+BDEI_time = namedtuple('BDEI_time', ['CPU_time', 'iterations'])
+
+
+def parse_tree(nwk):
+    """Parses an input tree in newick format and checks if it is binary and rooted"""
+    tree = None
+    for f in (0, 1, 2, 3, 5):
+        try:
+            tree = Tree(nwk, format=f)
+            break
+        except:
+            pass
+    if not tree:
+        raise ValueError("Please make sure to use correct newick format and to specify branch lengths.")
+    if len(tree.children) > 2:
+        raise ValueError("The input tree must be rooted and binary, please root your tree.")
+    for _ in tree.traverse():
+        n_children = len(_.children)
+        if not _.is_leaf() and n_children != 2:
+            raise ValueError("The input tree must be binary, while your tree contains internal nodes with {} children, "
+                             "please fix it.".format(n_children))
+        if not _.is_root() and _.dist == 0:
+            raise ValueError("The input tree must not contain non-root zero branches, while your tree does, "
+                             "please fix it.")
+    return tree
+
+
+def parse_forest(nwk):
+    res = []
+    with open(nwk, 'r') as f:
+        res = [parse_tree(_.strip('\n') + ';') for _ in f.read().split(';')[:-1]]
+    if not res:
+        raise ValueError('Could not find any trees in your input file (check the newick format): {}'.format(nwk))
+    return res
+
+
+def save_tree(tree, nwk):
+    with open(nwk, 'w+') as f:
+        f.write('{}\n'.format(tree.write(format=5, format_root_node=True)))
+
+
+def save_forest(forest, nwk):
+    with open(nwk, 'w+') as f:
+        for tree in forest:
+            _ = tree.write(format=5, format_root_node=True)
+            f.write('{}\n'.format(_))
+
+
+def initial_rate_guess(forest, mu=None, la=None, psi=None):
+
+    fixed_rates = []
+    for rate in (mu, la, psi):
+        if rate and rate > 0:
+            fixed_rates.append(rate)
+    if fixed_rates:
+        avg_rate = np.average(fixed_rates)
+        min_rate = avg_rate
+        max_rate = avg_rate
+    else:
+        internal_is, external_is = [], []
+        internal_es, external_es = [], []
+        for tree in forest:
+            for n in tree.traverse('preorder'):
+                if not n.is_leaf():
+                    i, e = sorted(n.children, key=lambda c: c.dist)
+                    (internal_is if not i.is_leaf() else external_is).append(i)
+                    (internal_es if not i.is_leaf() else external_es).append(e)
+        i_s_times = np.array([_.dist for _ in external_is])
+        i_tr_times = np.array([_.dist for _ in internal_is])
+        e_s_times = np.array([_.dist for _ in external_es])
+        e_tr_times = np.array([_.dist for _ in internal_es])
+        i_s_time = np.median(i_s_times)
+        e_s_time = np.median(e_s_times)
+        # if it is a corner case when we only have tips, let's use sampling times
+        i_tr_time = np.median(i_tr_times) if len(i_tr_times) else i_s_time
+        e_tr_time = np.median(e_tr_times) if len(e_tr_times) else e_s_time
+        mu_times = []
+        if e_s_time > i_s_time:
+            mu_times.append(e_s_time - i_s_time)
+        if e_tr_time > i_tr_time:
+            mu_times.append(e_tr_time - i_tr_time)
+        mu_time = np.average(mu_times) if mu_times else min(i_s_time, i_tr_time) * 0.01
+        avg_rate = np.average([1 / i_s_time, 1 / i_tr_time, 1 / mu_time])
+        min_rate = min([1 / i_s_time, 1 / i_tr_time, 1 / mu_time])
+        max_rate = max([1 / i_s_time, 1 / i_tr_time, 1 / mu_time])
+
+    return sorted({avg_rate, min_rate, max_rate})
+
+
+def infer(nwk, start=None, upper_bounds=None, pi_E=-1,
+          mu=-1, la=-1, psi=-1, p=-1, T=0.0, CI_repetitions=0, threads=1, log_level=INFO, **kwargs):
+    """Infer BDEI parameters from a phylogenetic tree."""
+
+    forest = None
+
+    if isinstance(start, BDEI_result):
+        start = np.array([start.mu, start.la, start.psi, start.p])
+    if start is None:
+        forest = parse_forest(nwk)
+        if not p or p <= 0 or p >= 1:
+            rate = initial_rate_guess(forest, mu, la, psi).pop()
+            starts = [[rate, rate, rate, pp] for pp in PS]
+        else:
+            starts = [[rate, rate, rate, p] for rate in initial_rate_guess(forest, mu, la, psi)]
+    else:
+        starts = [start]
+    for s in starts:
+        s[-1] = min(0.99, max(0.001, s[-1]))
+
+    if upper_bounds is None:
+        upper_bounds = np.array([np.inf, np.inf, np.inf, 1])
+    elif isinstance(upper_bounds, BDEI_result):
+        upper_bounds = np.array([upper_bounds.mu, upper_bounds.la, upper_bounds.psi, upper_bounds.p])
+    else:
+        upper_bounds = np.array(upper_bounds)
+    if any(upper_bounds <= 0):
+        raise ValueError('Upper bound must be positive.')
+    upper_bounds[-1] = min(upper_bounds[-1], 1)
+
+    if pi_E is not None and pi_E >= 0:
+        if pi_E > 1:
+            raise ValueError('Frequencies of pi_E should be between 0 and 1.')
+    else:
+        pi_E = -1
+
+    something_is_fixed = False
+    all_is_fixed = True
+    if mu >= 0:
+        upper_bounds[0] = mu
+        for s in starts:
+            s[0] = mu
+        something_is_fixed = True
+    else:
+        all_is_fixed = False
+    if la >= 0:
+        upper_bounds[1] = la
+        for s in starts:
+            s[1] = la
+        something_is_fixed = True
+    else:
+        all_is_fixed = False
+    if psi >= 0:
+        upper_bounds[2] = psi
+        for s in starts:
+            s[2] = psi
+        something_is_fixed = True
+    else:
+        all_is_fixed = False
+    if 0 < p <= 1:
+        upper_bounds[3] = p
+        for s in starts:
+            s[3] = p
+        something_is_fixed = True
+    else:
+        all_is_fixed = False
+
+    if not something_is_fixed:
+        raise ValueError('To be identifiable, the BDEI model needs one of its parameters to be fixed. '
+                         'Please do so, using one of the following arguments: mu, la, psi, p.')
+    if all_is_fixed:
+        raise ValueError('At least one of the following arguments: mu, la, psi, p, should be left to be optimised.')
+    starts = [np.minimum(s, upper_bounds * 0.999) for s in starts]
+    nstarts = len(starts)
+    starts = np.reshape(starts, (4 * nstarts,))
+
+    def get_res(_nwk):
+        return _pybdei.infer(f=_nwk, start=starts, ub=upper_bounds, pie=pi_E,
+                             mu=mu, la=la, psi=psi, p=p, T=T, nt=threads, nbiter=CI_repetitions,
+                             debug=log_level, nstarts=nstarts)
+
+    try:
+        res = get_res(nwk)
+    except:
+        temp_nwk = nwk + '.temp'
+        if forest is None:
+            forest = parse_forest(nwk)
+        save_forest(forest, temp_nwk)
+        res = get_res(temp_nwk)
+        try:
+            os.remove(temp_nwk)
+        except OSError:
+            pass
+
+    return BDEI_result(mu=res[0], la=res[1], psi=res[2], p=res[3],
+                       mu_CI=(res[4], res[5]) if CI_repetitions > 0 else None,
+                       la_CI=(res[6], res[7]) if CI_repetitions > 0 else None,
+                       psi_CI=(res[8], res[9]) if CI_repetitions > 0 else None,
+                       p_CI=(res[10], res[11]) if CI_repetitions > 0 else None,
+                       R_naught=res[1] / res[2], incubation_period=1 / res[0], infectious_time=1 / res[2]), \
+           BDEI_time(CPU_time=res[13], iterations=res[14])
+
+
+def get_loglikelihood(nwk, mu=-1, la=-1, psi=-1, p=-1, pi_E=-1, T=0.0, log_level=INFO, params=None, **kwargs):
+    """Calculate loglikelihood for given BDEI parameters from a phylogenetic tree."""
+    if params is not None:
+        if isinstance(params, BDEI_result):
+            mu = params.mu
+            la = params.la
+            psi = params.psi
+            p = params.p
+        else:
+            [mu, la, psi, p] = params
+    for par in [mu, la, psi, p]:
+        if par is None or par < 0:
+            raise ValueError('All the parameters (mu, la, psi, p) must be specified, '
+                             'either via dedicated arguments or via the params argument')
+
+    try:
+        res = _pybdei.likelihood(f=nwk, mu=mu, la=la, psi=psi, p=p, pie=pi_E, T=T, debug=log_level)
+    except:
+        temp_nwk = nwk + '.temp'
+        forest = parse_forest(nwk)
+        save_forest(forest, temp_nwk)
+        res = _pybdei.likelihood(f=temp_nwk, mu=mu, la=la, psi=psi, p=p, pie=pi_E, T=T, debug=log_level)
+        try:
+            os.remove(temp_nwk)
+        except OSError:
+            pass
+    return res
+
```

### Comparing `pybdei-0.4/pybdei/_pybdei.cpp` & `pybdei-0.5/pybdei/_pybdei.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,26 @@
     int nbiter = 0; //
     double p = -1;
     double la = -1;
     double mu = -1;
     double psi = -1;
     double pie = -1;
     double T = 0;
-    int u = 0;
     int nt = 0;
     int nstarts = 1;
     int debug = 2;
 
     PyObject *startobj, *ubobj;
 
     // Define keywords
-    static const char *kwlist[] = {"f", "start", "ub", "pie", "mu", "la", "psi", "p", "T", "u", "nt", "nbiter", "debug", "nstarts", NULL};
+    static const char *kwlist[] = {"f", "start", "ub", "pie", "mu", "la", "psi", "p", "T", "nt", "nbiter", "debug", "nstarts", NULL};
 
     // Interpret input arguments.
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "sOO|ddddddiiiii",
-        const_cast<char**>(kwlist), &treename, &startobj, &ubobj, &pie, &mu, &la, &psi, &p, &T, &u, &nt, &nbiter, &debug, &nstarts)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "sOO|ddddddiiii",
+        const_cast<char**>(kwlist), &treename, &startobj, &ubobj, &pie, &mu, &la, &psi, &p, &T, &nt, &nbiter, &debug, &nstarts)) {
         PyErr_Format(PyExc_ValueError, "Could not cast the input arguments.");
         return NULL;
     }
     // Interpret input objects as numpy arrays
     PyObject *startarray = PyArray_FROM_OTF(startobj, NPY_DOUBLE, NPY_ARRAY_IN_ARRAY);
     PyObject *ubarray = PyArray_FROM_OTF(ubobj, NPY_DOUBLE, NPY_ARRAY_IN_ARRAY);
     // If that didn't work, throw an exception
@@ -64,15 +63,15 @@
     PyArrayObject *ubarray_arr = reinterpret_cast<PyArrayObject*>(ubarray);
     double *ts = (double*)PyArray_DATA(startarray_arr);
     double *ubs = (double*)PyArray_DATA(ubarray_arr);
 
     PyObject *pysol = NULL;
     // Call the C++ functions to infer parameters
     try {
-        Solution sol = *inferParameters(treename, ts, ubs, pie, mu, la, psi, p, T, u, nbiter, nt, debug, nstarts);
+        Solution sol = *inferParameters(treename, ts, ubs, pie, mu, la, psi, p, T, nbiter, nt, debug, nstarts);
         pysol = PyList_New(15);
         PyList_SetItem(pysol, 0, Py_BuildValue("d", sol.mu));
         PyList_SetItem(pysol, 1, Py_BuildValue("d", sol.la));
         PyList_SetItem(pysol, 2, Py_BuildValue("d", sol.psi));
         PyList_SetItem(pysol, 3, Py_BuildValue("d", sol.p));
 
         PyList_SetItem(pysol, 4, Py_BuildValue("d", sol.mu_min));
@@ -108,29 +107,28 @@
     char* treename;
     double p = -1;
     double la = -1;
     double mu = -1;
     double psi = -1;
     double pie = -1;
     double T = 0;
-    int u = 0;
     int debug = 2;
 
     // Define keywords
-    static const char *kwlist[] = {"f", "mu", "la", "psi", "p", "pie", "T", "u", "debug", NULL};
+    static const char *kwlist[] = {"f", "mu", "la", "psi", "p", "pie", "T", "debug", NULL};
 
     // Interpret input arguments.
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "sddddddii",
-        const_cast<char**>(kwlist), &treename, &mu, &la, &psi, &p, &pie, &T, &u, &debug)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "sddddddi",
+        const_cast<char**>(kwlist), &treename, &mu, &la, &psi, &p, &pie, &T, &debug)) {
         PyErr_Format(PyExc_ValueError, "Could not cast the input arguments.");
         return NULL;
     }
 
     // Call the C++ functions to infer parameters
     try {
-        double res = calculateLikelihood(treename, mu, la, psi, p, pie, T, u, debug);
+        double res = calculateLikelihood(treename, mu, la, psi, p, pie, T, debug);
         return Py_BuildValue("d", res);
     } catch(const std::invalid_argument& e) {
         PyErr_SetString(PyExc_ValueError, e.what());
         return NULL;
     }
 }
```

### Comparing `pybdei-0.4/pybdei/_pybdei.hpp` & `pybdei-0.5/pybdei/_pybdei.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.4/pybdei/inference.py` & `pybdei-0.5/pybdei/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,14 @@
     import argparse
 
     parser = argparse.ArgumentParser(description="BDEI model parameter inference from phylogenetic trees.", prog='bdei_infer')
 
     tree_group = parser.add_argument_group('tree-related arguments')
     tree_group.add_argument('--nwk', help="Input tree(s) in newick format (must be rooted).",
                             type=str, required=True)
-    tree_group.add_argument('-u', '--u', help="Number of unobserved trees. "
-                                              "Can be non-zero only when all trees started at the same time "
-                                              "(i.e. T is given).",
-                            type=int, default=0)
 
     parameter_group = parser.add_argument_group('parameter-related arguments')
     parameter_group.add_argument('--mu', default=-1, type=float,
                                   help="Value to fix BDEI becoming-infectious rate mu. "
                                        "If not given, will be estimated.")
     parameter_group.add_argument('--la', default=-1, type=float,
                                   help="Value to fix BDEI transmission rate lambda. "
@@ -47,18 +43,15 @@
                                   help="Total time between the tree roots and the end of the epidemic "
                                        "(to be given if all trees start at the same time). "
                                        "If a positive value is given, the total time will be set to the maximum "
                                        "between this value and the maximal time between the start "
                                        "and the last sampled tip of all the trees. "
                                        "If a zero or negative value is given, the time will be tree-specific "
                                        "and estimated as the time between the root "
-                                       "and the last sampled tip for each tree."
-                                       "Note that if the number of unobserved trees (u) is given, "
-                                       "all the trees are assumed to have started at the same time, "
-                                       "hence T must be non-negative.")
+                                       "and the last sampled tip for each tree.")
 
     result_group = parser.add_argument_group('output-related arguments')
     result_group.add_argument('-c', '--CI_repetitions', default=0,
                               help="Number of repetitions for CI calculation "
                                    "(the higher, the more precise but also longer; a typical value is 100). "
                                    "If not specified, CIs will not be calculated.",
                               type=int)
```

### Comparing `pybdei-0.4/pybdei/loglikelihood.py` & `pybdei-0.5/pybdei/loglikelihood.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     import argparse
 
     parser = argparse.ArgumentParser(description="BDEI model parameter inference from phylogenetic trees.", prog='bdei_loglikelihood')
 
     tree_group = parser.add_argument_group('tree-related arguments')
     tree_group.add_argument('--nwk', help="input tree(s) in newick format (must be rooted).",
                             type=str, required=True)
-    tree_group.add_argument('-u', '--u', help="number of unobserved trees.",
-                            type=int, default=0)
 
     parameter_group = parser.add_argument_group('parameter-related arguments')
     parameter_group.add_argument('--mu', required=True, type=float, default=None,
                                   help="Value to fix BDEI becoming-infectious rate mu. "
                                        "If not given, will be estimated.")
     parameter_group.add_argument('--la', required=True, type=float, default=None,
                                   help="Value to fix BDEI transmission rate lambda. "
@@ -37,18 +35,15 @@
                                   help="Total time between the tree roots and the end of the epidemic "
                                        "(to be given if all trees start at the same time). "
                                        "If a positive value is given, the total time will be set to the maximum "
                                        "between this value and the maximal time between the start "
                                        "and the last sampled tip of all the trees. "
                                        "If a zero or negative value is given, the time will be tree-specific "
                                        "and estimated as the time between the root "
-                                       "and the last sampled tip for each tree."
-                                       "Note that if the number of unobserved trees (u) is given, "
-                                       "all the trees are assumed to have started at the same time, "
-                                       "hence T must be non-negative.")
+                                       "and the last sampled tip for each tree.")
     parser.add_argument('--log_level',
                         help="level of logging information "
                              "(the lower, the less information will be printed to the output). "
                              "Possible levels are: {} (errors only), {} (errors+warnings), {} (errors+warnings+info), "
                              "{} (errors+warnings+info+debug).".format(ERRORS, WARNINGS, INFO, DEBUG), type=int,
                         default=INFO)
     parser.add_argument('-v', '--version', action='version', version='%(prog)s {version}'.format(version=PYBDEI_VERSION))
```

### Comparing `pybdei-0.4/pybdei.egg-info/PKG-INFO` & `pybdei-0.5/pybdei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdei
-Version: 0.4
+Version: 0.5
 Summary: Fast and accurate epidemiological parameter estimation from phylogenetic trees with the Birth-Death Exposed-Infectious (BDEI) model.
 Home-page: https://github.com/evolbioinfo/BDEI
 Download-URL: https://github.com/evolbioinfo/BDEI
 Author: Frédéric Heicht
 Author-email: frederic.hecht@sorbonne-universite.fr
 Maintainer: Anna Zhukova
 Maintainer-email: anna.zhukova@pasteur.fr
```

### Comparing `pybdei-0.4/setup.py` & `pybdei-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ],
     packages=find_packages(),
     install_requires=['numpy', 'ete3', 'six'],
     setup_requires=['numpy'],
     include_package_data=True,
     package_data={'pybdei': ['*.hpp'],
                   'bdei': ['*.hpp']},
-    version='0.4',
+    version='0.5',
     description='Fast and accurate epidemiological parameter estimation from phylogenetic trees with the Birth-Death Exposed-Infectious (BDEI) model.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Frédéric Heicht',
     author_email='frederic.hecht@sorbonne-universite.fr',
     maintainer='Anna Zhukova',
     maintainer_email='anna.zhukova@pasteur.fr',
```

