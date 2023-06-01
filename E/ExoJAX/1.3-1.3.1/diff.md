# Comparing `tmp/ExoJAX-1.3-py3.8.egg` & `tmp/ExoJAX-1.3.1-py3.8.egg`

## zipinfo {}

```diff
@@ -1,53 +1,57 @@
-Zip file size: 6802530 bytes, number of entries: 275
--rw-rw-r--  2.0 unx     4671 b- defN 23-Mar-15 18:44 EGG-INFO/PKG-INFO
--rw-rw-r--  2.0 unx   161090 b- defN 23-Mar-15 18:44 EGG-INFO/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-15 18:44 EGG-INFO/dependency_links.txt
+Zip file size: 6822352 bytes, number of entries: 295
+-rw-rw-r--  2.0 unx     4673 b- defN 23-Jun-01 18:04 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx   161923 b- defN 23-Jun-01 18:04 EGG-INFO/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-01 18:04 EGG-INFO/dependency_links.txt
 -rw-rw-r--  2.0 unx        1 b- defN 22-Nov-10 18:19 EGG-INFO/not-zip-safe
--rw-rw-r--  2.0 unx       71 b- defN 23-Mar-15 18:44 EGG-INFO/requires.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-15 18:44 EGG-INFO/top_level.txt
--rw-rw-r--  2.0 unx      298 b- defN 22-May-01 08:50 exojax/__init__.py
--rw-rw-r--  2.0 unx      456 b- defN 23-Mar-15 18:44 exojax/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx       71 b- defN 23-Jun-01 18:04 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-01 18:04 EGG-INFO/top_level.txt
+-rw-rw-r--  2.0 unx      298 b- defN 23-Jun-01 17:59 exojax/__init__.py
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Apr-09 09:40 exojax/data.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Apr-09 09:41 exojax/emulate_broadpar.py
+-rw-rw-r--  2.0 unx      456 b- defN 23-Jun-01 18:04 exojax/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1620 b- defN 23-Jun-01 18:04 exojax/__pycache__/data.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1137 b- defN 23-Jun-01 18:04 exojax/__pycache__/emulate_broadpar.cpython-38.pyc
 -rw-rw-r--  2.0 unx      213 b- defN 22-May-01 08:50 exojax/atm/__init__.py
 -rw-rw-r--  2.0 unx     3023 b- defN 22-May-01 08:50 exojax/atm/amclouds.py
--rw-rw-r--  2.0 unx     2719 b- defN 23-Mar-15 18:34 exojax/atm/atmprof.py
+-rw-rw-r--  2.0 unx     2719 b- defN 23-Jun-01 17:59 exojax/atm/atmprof.py
 -rw-rw-r--  2.0 unx      676 b- defN 22-May-01 08:50 exojax/atm/condinfo.py
 -rw-rw-r--  2.0 unx    10719 b- defN 22-Oct-26 08:56 exojax/atm/fastchem2_call.py
 -rw-rw-r--  2.0 unx      315 b- defN 22-May-01 08:50 exojax/atm/idealgas.py
 -rw-rw-r--  2.0 unx      972 b- defN 22-May-01 08:50 exojax/atm/psat.py
 -rw-rw-r--  2.0 unx      434 b- defN 22-May-01 08:50 exojax/atm/simple_clouds.py
 -rw-rw-r--  2.0 unx     3002 b- defN 23-Mar-15 18:34 exojax/atm/viscosity.py
 -rw-rw-r--  2.0 unx     4056 b- defN 22-May-01 08:50 exojax/atm/vterm.py
--rw-rw-r--  2.0 unx      373 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     3462 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/amclouds.cpython-38.pyc
--rw-rw-r--  2.0 unx     3254 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/atmprof.cpython-38.pyc
--rw-rw-r--  2.0 unx      717 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/condinfo.cpython-38.pyc
--rw-rw-r--  2.0 unx     9208 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/fastchem2_call.cpython-38.pyc
--rw-rw-r--  2.0 unx      538 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/idealgas.cpython-38.pyc
--rw-rw-r--  2.0 unx     1354 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/psat.cpython-38.pyc
--rw-rw-r--  2.0 unx      668 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/simple_clouds.cpython-38.pyc
--rw-rw-r--  2.0 unx     2891 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/viscosity.cpython-38.pyc
--rw-rw-r--  2.0 unx     4656 b- defN 23-Mar-15 18:44 exojax/atm/__pycache__/vterm.cpython-38.pyc
+-rw-rw-r--  2.0 unx      373 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3462 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/amclouds.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3254 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/atmprof.cpython-38.pyc
+-rw-rw-r--  2.0 unx      717 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/condinfo.cpython-38.pyc
+-rw-rw-r--  2.0 unx     9208 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/fastchem2_call.cpython-38.pyc
+-rw-rw-r--  2.0 unx      538 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/idealgas.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1354 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/psat.cpython-38.pyc
+-rw-rw-r--  2.0 unx      668 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/simple_clouds.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2891 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/viscosity.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4656 b- defN 23-Jun-01 18:04 exojax/atm/__pycache__/vterm.cpython-38.pyc
 -rw-rw-r--  2.0 unx      171 b- defN 22-May-01 08:50 exojax/data/__init__.py
--rw-rw-r--  2.0 unx      332 b- defN 23-Mar-15 18:44 exojax/data/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx      332 b- defN 23-Jun-01 18:04 exojax/data/__pycache__/__init__.cpython-38.pyc
 -rw-rw-r--  2.0 unx     2403 b- defN 22-May-01 08:50 exojax/data/abundance/AAG2021.dat
 -rw-rw-r--  2.0 unx     9614 b- defN 23-Feb-06 22:31 exojax/data/atom/HITRAN_molparam.txt
 -rw-rw-r--  2.0 unx   819291 b- defN 22-May-01 08:50 exojax/data/atom/NIST_Atomic_Ionization_Energies.txt
 -rw-rw-r--  2.0 unx     6044 b- defN 22-May-01 08:50 exojax/data/atom/atomic.txt
 -rw-rw-r--  2.0 unx   171536 b- defN 22-May-01 08:50 exojax/data/atom/barklem_collet_2016_pff.txt
 -rw-rw-r--  2.0 unx     8322 b- defN 22-May-01 08:50 exojax/data/atom/iso_mn.txt
 -rw-rw-r--  2.0 unx      188 b- defN 22-May-01 08:50 exojax/data/clouds/drag_force.txt
 -rw-rw-r--  2.0 unx  3483224 b- defN 23-Mar-15 18:34 exojax/data/premodit/elower_grid_trange.npz
 -rw-rw-r--  2.0 unx     2300 b- defN 23-Mar-15 18:34 exojax/data/testdata/H2-H2_TEST.cia
--rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/lpf_rt_test_hitemp_ref.txt
--rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/lpf_rt_test_ref.txt
+-rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-19 10:35 exojax/data/testdata/lpf_rt_test_hitemp_ref.txt
+-rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-19 10:35 exojax/data/testdata/lpf_rt_test_ref.txt
 -rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/lpf_test_hitemp_ref.txt
 -rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/lpf_test_ref.txt
--rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/modit_rt_test_hitemp_ref.txt
--rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/modit_rt_test_ref.txt
+-rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-19 10:35 exojax/data/testdata/modit_rt_test_hitemp_ref.txt
+-rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-19 10:35 exojax/data/testdata/modit_rt_test_ref.txt
 -rw-rw-r--  2.0 unx   100000 b- defN 23-Feb-06 22:31 exojax/data/testdata/modit_rt_test_vald_ref.txt
 -rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/modit_test_hitemp_ref.txt
 -rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/modit_test_hitemp_ref_air.txt
 -rw-rw-r--  2.0 unx  1000000 b- defN 23-Mar-15 18:34 exojax/data/testdata/modit_test_ref.txt
 -rw-rw-r--  2.0 unx   157039 b- defN 23-Feb-10 19:51 exojax/data/testdata/moldb_co_exomol.pickle
 -rw-rw-r--  2.0 unx    49346 b- defN 23-Feb-10 19:51 exojax/data/testdata/moldb_co_hitemp.pickle
 -rw-rw-r--  2.0 unx    16092 b- defN 23-Feb-10 19:51 exojax/data/testdata/moldb_co_hitemp_single_isotope.pickle
@@ -55,223 +59,239 @@
 -rw-rw-r--  2.0 unx   151554 b- defN 23-Feb-07 10:52 exojax/data/testdata/moldb_vald.pickle
 -rw-rw-r--  2.0 unx   750000 b- defN 23-Feb-06 22:31 exojax/data/testdata/premodit_rt_test_hitemp_ref.txt
 -rw-rw-r--  2.0 unx   750000 b- defN 22-Dec-07 21:18 exojax/data/testdata/premodit_rt_test_ref.txt
 -rw-rw-r--  2.0 unx   250000 b- defN 23-Feb-06 22:31 exojax/data/testdata/premodit_test_hitemp_ref.txt
 -rw-rw-r--  2.0 unx   250000 b- defN 22-Dec-07 21:18 exojax/data/testdata/premodit_test_ref.txt
 -rw-rw-r--  2.0 unx    25000 b- defN 22-May-24 15:32 exojax/data/testdata/spectrum.txt
 -rw-rw-r--  2.0 unx    75000 b- defN 22-Dec-07 21:18 exojax/data/testdata/spectrum_ch4.txt
--rw-rw-r--  2.0 unx    75000 b- defN 23-Mar-15 18:34 exojax/data/testdata/spectrum_ch4_new.txt
+-rw-rw-r--  2.0 unx    75000 b- defN 23-Mar-19 10:35 exojax/data/testdata/spectrum_ch4_new.txt
 -rw-rw-r--  2.0 unx    75000 b- defN 22-Dec-07 21:18 exojax/data/testdata/spectrum_co.txt
 -rw-rw-r--  2.0 unx  2104704 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/05_HITEMP_SAMPLE.par
 -rw-rw-r--  2.0 unx     1944 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__H2.broad
 -rw-rw-r--  2.0 unx     1680 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__He.broad
 -rw-rw-r--  2.0 unx     5074 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.def
 -rw-rw-r--  2.0 unx   234000 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.pf
 -rw-rw-r--  2.0 unx    54318 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.bz2
 -rw-rw-r--  2.0 unx   217080 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.hdf5
 -rw-rw-r--  2.0 unx     3105 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.bz2
 -rw-rw-r--  2.0 unx   134416 b- defN 23-Mar-15 18:34 exojax/data/testdata/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.hdf5
 -rw-rw-r--  2.0 unx      167 b- defN 22-May-01 08:50 exojax/dynamics/__init__.py
 -rw-rw-r--  2.0 unx     2646 b- defN 23-Feb-06 22:31 exojax/dynamics/getE.py
 -rw-rw-r--  2.0 unx     2806 b- defN 23-Feb-06 22:31 exojax/dynamics/rvfunc.py
--rw-rw-r--  2.0 unx      330 b- defN 23-Mar-15 18:44 exojax/dynamics/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     3601 b- defN 23-Mar-15 18:44 exojax/dynamics/__pycache__/getE.cpython-38.pyc
--rw-rw-r--  2.0 unx     3314 b- defN 23-Mar-15 18:44 exojax/dynamics/__pycache__/rvfunc.cpython-38.pyc
+-rw-rw-r--  2.0 unx      330 b- defN 23-Jun-01 18:04 exojax/dynamics/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3601 b- defN 23-Jun-01 18:04 exojax/dynamics/__pycache__/getE.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3314 b- defN 23-Jun-01 18:04 exojax/dynamics/__pycache__/rvfunc.cpython-38.pyc
 -rw-rw-r--  2.0 unx      255 b- defN 22-May-01 08:50 exojax/plot/__init__.py
 -rw-rw-r--  2.0 unx     5963 b- defN 23-Feb-06 22:31 exojax/plot/atmplot.py
 -rw-rw-r--  2.0 unx     2124 b- defN 22-May-01 08:50 exojax/plot/ditplot.py
--rw-rw-r--  2.0 unx      427 b- defN 23-Mar-15 18:44 exojax/plot/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     5347 b- defN 23-Mar-15 18:44 exojax/plot/__pycache__/atmplot.cpython-38.pyc
--rw-rw-r--  2.0 unx     2209 b- defN 23-Mar-15 18:44 exojax/plot/__pycache__/ditplot.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1507 b- defN 23-May-20 12:49 exojax/plot/opaplot.py
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jun-01 18:04 exojax/plot/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5347 b- defN 23-Jun-01 18:04 exojax/plot/__pycache__/atmplot.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2209 b- defN 23-Jun-01 18:04 exojax/plot/__pycache__/ditplot.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1463 b- defN 23-Jun-01 18:04 exojax/plot/__pycache__/opaplot.cpython-38.pyc
 -rw-rw-r--  2.0 unx       65 b- defN 23-Feb-06 22:31 exojax/signal/__init__.py
 -rw-rw-r--  2.0 unx      698 b- defN 23-Mar-15 18:34 exojax/signal/convolve.py
 -rw-rw-r--  2.0 unx     6552 b- defN 23-Mar-02 07:26 exojax/signal/ola.py
--rw-rw-r--  2.0 unx      215 b- defN 23-Mar-15 18:44 exojax/signal/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx      800 b- defN 23-Mar-15 18:44 exojax/signal/__pycache__/convolve.cpython-38.pyc
--rw-rw-r--  2.0 unx     6275 b- defN 23-Mar-15 18:44 exojax/signal/__pycache__/ola.cpython-38.pyc
--rw-rw-r--  2.0 unx      484 b- defN 23-Mar-15 18:34 exojax/spec/__init__.py
--rw-rw-r--  2.0 unx    39886 b- defN 23-Mar-15 18:34 exojax/spec/api.py
+-rw-rw-r--  2.0 unx      215 b- defN 23-Jun-01 18:04 exojax/signal/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx      800 b- defN 23-Jun-01 18:04 exojax/signal/__pycache__/convolve.cpython-38.pyc
+-rw-rw-r--  2.0 unx     6275 b- defN 23-Jun-01 18:04 exojax/signal/__pycache__/ola.cpython-38.pyc
+-rw-rw-r--  2.0 unx      484 b- defN 23-Mar-19 10:35 exojax/spec/__init__.py
+-rw-rw-r--  2.0 unx    39886 b- defN 23-Jun-01 17:59 exojax/spec/api.py
 -rw-rw-r--  2.0 unx    36096 b- defN 23-Feb-04 11:33 exojax/spec/api_current.py
--rw-rw-r--  2.0 unx     6910 b- defN 23-Mar-15 18:34 exojax/spec/atmrt.py
+-rw-rw-r--  2.0 unx     6910 b- defN 23-Jun-01 17:59 exojax/spec/atmrt.py
 -rw-rw-r--  2.0 unx    28504 b- defN 23-Mar-15 18:34 exojax/spec/atomll.py
 -rw-rw-r--  2.0 unx    16617 b- defN 23-Feb-06 22:31 exojax/spec/atomllapi.py
 -rw-rw-r--  2.0 unx    18373 b- defN 23-Mar-15 08:00 exojax/spec/autospec.py
 -rw-rw-r--  2.0 unx     3004 b- defN 22-Oct-26 08:56 exojax/spec/check_nugrid.py
 -rw-rw-r--  2.0 unx     1637 b- defN 22-May-24 15:32 exojax/spec/contdb.py
 -rw-rw-r--  2.0 unx     1682 b- defN 22-May-01 08:50 exojax/spec/defcia.py
 -rw-rw-r--  2.0 unx     3707 b- defN 23-Feb-10 20:28 exojax/spec/defmol.py
--rw-rw-r--  2.0 unx    11359 b- defN 23-Mar-15 18:34 exojax/spec/dit.py
+-rw-rw-r--  2.0 unx    11359 b- defN 23-Mar-19 10:35 exojax/spec/dit.py
 -rw-rw-r--  2.0 unx     4499 b- defN 23-Feb-06 22:31 exojax/spec/ditkernel.py
--rw-rw-r--  2.0 unx     3560 b- defN 23-Mar-12 07:28 exojax/spec/dtau_mmwl.py
+-rw-rw-r--  2.0 unx     3560 b- defN 23-Apr-05 20:12 exojax/spec/dtau_mmwl.py
 -rw-rw-r--  2.0 unx     6071 b- defN 22-May-01 08:50 exojax/spec/evalline.py
 -rw-rw-r--  2.0 unx     1340 b- defN 22-May-01 08:50 exojax/spec/exomol.py
 -rw-rw-r--  2.0 unx    15387 b- defN 23-Feb-10 19:51 exojax/spec/exomolapi.py
 -rw-rw-r--  2.0 unx  1267866 b- defN 22-Aug-25 16:22 exojax/spec/hapi.py
--rw-rw-r--  2.0 unx     3546 b- defN 23-Mar-15 18:34 exojax/spec/hitran.py
+-rw-rw-r--  2.0 unx     3546 b- defN 23-Mar-19 10:35 exojax/spec/hitran.py
 -rw-rw-r--  2.0 unx     1916 b- defN 23-Mar-15 18:34 exojax/spec/hitranapi.py
 -rw-rw-r--  2.0 unx     3357 b- defN 23-Mar-15 18:34 exojax/spec/hitrancia.py
 -rw-rw-r--  2.0 unx     5845 b- defN 22-May-01 08:50 exojax/spec/hminus.py
--rw-rw-r--  2.0 unx     9355 b- defN 23-Mar-15 18:34 exojax/spec/initspec.py
--rw-rw-r--  2.0 unx     3899 b- defN 23-Mar-12 07:55 exojax/spec/layeropacity.py
+-rw-rw-r--  2.0 unx     9355 b- defN 23-Jun-01 17:59 exojax/spec/initspec.py
+-rw-rw-r--  2.0 unx     4219 b- defN 23-Apr-05 20:12 exojax/spec/layeropacity.py
 -rw-rw-r--  2.0 unx     3979 b- defN 23-Mar-15 18:34 exojax/spec/lbd.py
 -rw-rw-r--  2.0 unx     9993 b- defN 23-Mar-15 18:34 exojax/spec/lbderror.py
 -rw-rw-r--  2.0 unx      405 b- defN 23-Feb-06 22:31 exojax/spec/limb_darkening.py
 -rw-rw-r--  2.0 unx      121 b- defN 22-Sep-08 18:15 exojax/spec/linefilter.py
--rw-rw-r--  2.0 unx    12592 b- defN 23-Mar-15 18:34 exojax/spec/lpf.py
+-rw-rw-r--  2.0 unx    12592 b- defN 23-Mar-19 10:35 exojax/spec/lpf.py
 -rw-rw-r--  2.0 unx     8566 b- defN 23-Mar-15 18:34 exojax/spec/lsd.py
--rw-rw-r--  2.0 unx     3836 b- defN 23-Feb-06 22:31 exojax/spec/make_numatrix.py
--rw-rw-r--  2.0 unx    25279 b- defN 23-Mar-15 18:34 exojax/spec/modit.py
--rw-rw-r--  2.0 unx     5095 b- defN 23-Feb-13 11:26 exojax/spec/modit_scanfft.py
+-rw-rw-r--  2.0 unx     3836 b- defN 23-Jun-01 17:59 exojax/spec/make_numatrix.py
+-rw-rw-r--  2.0 unx    25279 b- defN 23-Mar-19 10:35 exojax/spec/modit.py
+-rw-rw-r--  2.0 unx     5095 b- defN 23-Apr-02 08:50 exojax/spec/modit_scanfft.py
 -rw-rw-r--  2.0 unx    24097 b- defN 23-Mar-15 18:34 exojax/spec/moldb.py
 -rw-rw-r--  2.0 unx    62169 b- defN 23-Mar-15 08:00 exojax/spec/moldf.py
 -rw-rw-r--  2.0 unx     5970 b- defN 23-Mar-15 18:34 exojax/spec/molinfo.py
--rw-rw-r--  2.0 unx    19215 b- defN 23-Mar-15 18:34 exojax/spec/opacalc.py
--rw-rw-r--  2.0 unx     1248 b- defN 23-Mar-12 06:51 exojax/spec/opachord.py
+-rw-rw-r--  2.0 unx     2320 b- defN 23-May-13 21:25 exojax/spec/nonair.py
+-rw-rw-r--  2.0 unx    19215 b- defN 23-Jun-01 17:59 exojax/spec/opacalc.py
+-rw-rw-r--  2.0 unx     1668 b- defN 23-Apr-05 20:12 exojax/spec/opachord.py
 -rw-rw-r--  2.0 unx     3123 b- defN 22-Aug-25 12:34 exojax/spec/opacity.py
 -rw-rw-r--  2.0 unx      847 b- defN 23-Feb-06 22:31 exojax/spec/opacitytools.py
 -rw-rw-r--  2.0 unx     1197 b- defN 23-Mar-15 18:34 exojax/spec/opacont.py
--rw-rw-r--  2.0 unx     3438 b- defN 23-Mar-15 18:34 exojax/spec/optgrid.py
+-rw-rw-r--  2.0 unx     1110 b- defN 23-Apr-12 12:49 exojax/spec/opspec.py
+-rw-rw-r--  2.0 unx     3438 b- defN 23-Jun-01 17:59 exojax/spec/optgrid.py
 -rw-rw-r--  2.0 unx      663 b- defN 22-May-01 08:50 exojax/spec/planck.py
 -rw-rw-r--  2.0 unx    21807 b- defN 23-Mar-15 08:00 exojax/spec/plg.py
--rw-rw-r--  2.0 unx    22792 b- defN 23-Mar-15 18:34 exojax/spec/premodit.py
+-rw-rw-r--  2.0 unx    22792 b- defN 23-Jun-01 17:59 exojax/spec/premodit.py
 -rw-rw-r--  2.0 unx     3295 b- defN 23-Mar-02 07:26 exojax/spec/presolar.py
 -rw-rw-r--  2.0 unx       91 b- defN 23-Feb-28 11:56 exojax/spec/presolar_scanola.py
+-rw-rw-r--  2.0 unx      399 b- defN 23-May-13 21:25 exojax/spec/qstate.py
 -rw-rw-r--  2.0 unx      164 b- defN 22-Jul-13 14:12 exojax/spec/radis_test.py
--rw-rw-r--  2.0 unx     3364 b- defN 23-Mar-15 18:34 exojax/spec/response.py
+-rw-rw-r--  2.0 unx     3364 b- defN 23-Jun-01 17:59 exojax/spec/response.py
 -rw-rw-r--  2.0 unx     1384 b- defN 22-Oct-26 08:56 exojax/spec/rtcheck.py
--rw-rw-r--  2.0 unx    10477 b- defN 23-Mar-15 18:34 exojax/spec/rtransfer.py
--rw-rw-r--  2.0 unx     5466 b- defN 22-Dec-07 21:18 exojax/spec/set_ditgrid.py
+-rw-rw-r--  2.0 unx    10477 b- defN 23-Jun-01 17:59 exojax/spec/rtransfer.py
+-rw-rw-r--  2.0 unx     5467 b- defN 23-Jun-01 17:59 exojax/spec/set_ditgrid.py
 -rw-rw-r--  2.0 unx     1325 b- defN 22-May-27 16:48 exojax/spec/set_ditgrid_matrix.py
 -rw-rw-r--  2.0 unx     4168 b- defN 22-May-27 16:29 exojax/spec/setdit.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Oct-16 10:41 exojax/spec/setrt.py
 -rw-rw-r--  2.0 unx     1700 b- defN 23-Feb-06 22:31 exojax/spec/shapefilter.py
+-rw-rw-r--  2.0 unx     3237 b- defN 23-Apr-14 09:59 exojax/spec/specop.py
 -rw-rw-r--  2.0 unx     2185 b- defN 23-Mar-15 18:34 exojax/spec/spin_rotation.py
 -rw-rw-r--  2.0 unx      847 b- defN 22-Oct-26 08:56 exojax/spec/tau1height.py
--rw-rw-r--  2.0 unx      727 b- defN 23-Mar-15 18:28 exojax/spec/unitconvert.py
--rw-rw-r--  2.0 unx      672 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx    28487 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/api.cpython-38.pyc
--rw-rw-r--  2.0 unx    27013 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/api_current.cpython-38.pyc
--rw-rw-r--  2.0 unx     7345 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/atmrt.cpython-38.pyc
--rw-rw-r--  2.0 unx    25836 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/atomll.cpython-38.pyc
--rw-rw-r--  2.0 unx    14758 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/atomllapi.cpython-38.pyc
--rw-rw-r--  2.0 unx    13563 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/autospec.cpython-38.pyc
--rw-rw-r--  2.0 unx     3011 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/check_nugrid.cpython-38.pyc
--rw-rw-r--  2.0 unx     1918 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/contdb.cpython-38.pyc
--rw-rw-r--  2.0 unx     1689 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/defcia.cpython-38.pyc
--rw-rw-r--  2.0 unx     2311 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/defmol.cpython-38.pyc
--rw-rw-r--  2.0 unx    10820 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/dit.cpython-38.pyc
--rw-rw-r--  2.0 unx     4486 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/ditkernel.cpython-38.pyc
--rw-rw-r--  2.0 unx     3522 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/dtau_mmwl.cpython-38.pyc
--rw-rw-r--  2.0 unx     5770 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/evalline.cpython-38.pyc
--rw-rw-r--  2.0 unx     1659 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/exomol.cpython-38.pyc
--rw-rw-r--  2.0 unx    12167 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/exomolapi.cpython-38.pyc
--rw-rw-r--  2.0 unx  1043677 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/hapi.cpython-38.pyc
--rw-rw-r--  2.0 unx     3658 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/hitran.cpython-38.pyc
--rw-rw-r--  2.0 unx     1863 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/hitranapi.cpython-38.pyc
--rw-rw-r--  2.0 unx     3491 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/hitrancia.cpython-38.pyc
--rw-rw-r--  2.0 unx     5093 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/hminus.cpython-38.pyc
--rw-rw-r--  2.0 unx     8536 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/initspec.cpython-38.pyc
--rw-rw-r--  2.0 unx     3932 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/layeropacity.cpython-38.pyc
--rw-rw-r--  2.0 unx     3362 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/lbd.cpython-38.pyc
--rw-rw-r--  2.0 unx     8818 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/lbderror.cpython-38.pyc
--rw-rw-r--  2.0 unx      638 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/limb_darkening.cpython-38.pyc
--rw-rw-r--  2.0 unx      329 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/linefilter.cpython-38.pyc
--rw-rw-r--  2.0 unx    11668 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/lpf.cpython-38.pyc
--rw-rw-r--  2.0 unx     7856 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/lsd.cpython-38.pyc
--rw-rw-r--  2.0 unx     3977 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/make_numatrix.cpython-38.pyc
--rw-rw-r--  2.0 unx    21780 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/modit.cpython-38.pyc
--rw-rw-r--  2.0 unx     5142 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/modit_scanfft.cpython-38.pyc
--rw-rw-r--  2.0 unx    19163 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/moldb.cpython-38.pyc
--rw-rw-r--  2.0 unx    43035 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/moldf.cpython-38.pyc
--rw-rw-r--  2.0 unx     4935 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/molinfo.cpython-38.pyc
--rw-rw-r--  2.0 unx    14158 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/opacalc.cpython-38.pyc
--rw-rw-r--  2.0 unx     1395 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/opachord.cpython-38.pyc
--rw-rw-r--  2.0 unx     2886 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/opacity.cpython-38.pyc
--rw-rw-r--  2.0 unx     1071 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/opacitytools.cpython-38.pyc
--rw-rw-r--  2.0 unx     1641 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/opacont.cpython-38.pyc
--rw-rw-r--  2.0 unx     2849 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/optgrid.cpython-38.pyc
--rw-rw-r--  2.0 unx      907 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/planck.cpython-38.pyc
--rw-rw-r--  2.0 unx    17342 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/plg.cpython-38.pyc
--rw-rw-r--  2.0 unx    17972 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/premodit.cpython-38.pyc
--rw-rw-r--  2.0 unx     3342 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/presolar.cpython-38.pyc
--rw-rw-r--  2.0 unx      318 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/presolar_scanola.cpython-38.pyc
--rw-rw-r--  2.0 unx      331 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/radis_test.cpython-38.pyc
--rw-rw-r--  2.0 unx     3800 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/response.cpython-38.pyc
--rw-rw-r--  2.0 unx     1757 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/rtcheck.cpython-38.pyc
--rw-rw-r--  2.0 unx    10095 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/rtransfer.cpython-38.pyc
--rw-rw-r--  2.0 unx     5175 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/set_ditgrid.cpython-38.pyc
--rw-rw-r--  2.0 unx     1416 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/set_ditgrid_matrix.cpython-38.pyc
--rw-rw-r--  2.0 unx     4048 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/setdit.cpython-38.pyc
--rw-rw-r--  2.0 unx      521 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/setrt.cpython-38.pyc
--rw-rw-r--  2.0 unx     1901 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/shapefilter.cpython-38.pyc
--rw-rw-r--  2.0 unx     2153 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/spin_rotation.cpython-38.pyc
--rw-rw-r--  2.0 unx     1069 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/tau1height.cpython-38.pyc
--rw-rw-r--  2.0 unx      925 b- defN 23-Mar-15 18:44 exojax/spec/__pycache__/unitconvert.cpython-38.pyc
+-rw-rw-r--  2.0 unx      727 b- defN 23-Jun-01 17:59 exojax/spec/unitconvert.py
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx    28487 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/api.cpython-38.pyc
+-rw-rw-r--  2.0 unx    27013 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/api_current.cpython-38.pyc
+-rw-rw-r--  2.0 unx     7345 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/atmrt.cpython-38.pyc
+-rw-rw-r--  2.0 unx    25836 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/atomll.cpython-38.pyc
+-rw-rw-r--  2.0 unx    14758 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/atomllapi.cpython-38.pyc
+-rw-rw-r--  2.0 unx    13563 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/autospec.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3011 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/check_nugrid.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1918 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/contdb.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1689 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/defcia.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2311 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/defmol.cpython-38.pyc
+-rw-rw-r--  2.0 unx    10820 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/dit.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4486 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/ditkernel.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3522 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/dtau_mmwl.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5770 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/evalline.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1659 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/exomol.cpython-38.pyc
+-rw-rw-r--  2.0 unx    12167 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/exomolapi.cpython-38.pyc
+-rw-rw-r--  2.0 unx  1043677 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/hapi.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3658 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/hitran.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1863 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/hitranapi.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3491 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/hitrancia.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5093 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/hminus.cpython-38.pyc
+-rw-rw-r--  2.0 unx     8536 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/initspec.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4129 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/layeropacity.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3362 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/lbd.cpython-38.pyc
+-rw-rw-r--  2.0 unx     8818 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/lbderror.cpython-38.pyc
+-rw-rw-r--  2.0 unx      638 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/limb_darkening.cpython-38.pyc
+-rw-rw-r--  2.0 unx      329 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/linefilter.cpython-38.pyc
+-rw-rw-r--  2.0 unx    11668 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/lpf.cpython-38.pyc
+-rw-rw-r--  2.0 unx     7856 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/lsd.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3977 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/make_numatrix.cpython-38.pyc
+-rw-rw-r--  2.0 unx    21780 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/modit.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5142 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/modit_scanfft.cpython-38.pyc
+-rw-rw-r--  2.0 unx    19163 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/moldb.cpython-38.pyc
+-rw-rw-r--  2.0 unx    43035 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/moldf.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4935 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/molinfo.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2311 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/nonair.cpython-38.pyc
+-rw-rw-r--  2.0 unx    14158 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/opacalc.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1796 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/opachord.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2886 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/opacity.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1071 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/opacitytools.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1641 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/opacont.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/opspec.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2849 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/optgrid.cpython-38.pyc
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/planck.cpython-38.pyc
+-rw-rw-r--  2.0 unx    17342 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/plg.cpython-38.pyc
+-rw-rw-r--  2.0 unx    17972 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/premodit.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3342 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/presolar.cpython-38.pyc
+-rw-rw-r--  2.0 unx      318 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/presolar_scanola.cpython-38.pyc
+-rw-rw-r--  2.0 unx      601 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/qstate.cpython-38.pyc
+-rw-rw-r--  2.0 unx      331 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/radis_test.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3800 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/response.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1757 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/rtcheck.cpython-38.pyc
+-rw-rw-r--  2.0 unx    10095 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/rtransfer.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5075 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/set_ditgrid.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/set_ditgrid_matrix.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4048 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/setdit.cpython-38.pyc
+-rw-rw-r--  2.0 unx      521 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/setrt.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1901 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/shapefilter.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3725 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/specop.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/spin_rotation.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/tau1height.cpython-38.pyc
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-01 18:04 exojax/spec/__pycache__/unitconvert.cpython-38.pyc
 -rw-rw-r--  2.0 unx      345 b- defN 23-Feb-06 22:31 exojax/special/__init__.py
 -rw-rw-r--  2.0 unx    10399 b- defN 22-Sep-18 13:27 exojax/special/_special.py
 -rw-rw-r--  2.0 unx     1067 b- defN 23-Feb-06 22:31 exojax/special/erfcx.py
 -rw-rw-r--  2.0 unx      836 b- defN 22-Sep-06 07:10 exojax/special/expn.py
 -rw-rw-r--  2.0 unx     3939 b- defN 23-Feb-06 22:31 exojax/special/faddeeva.py
 -rw-rw-r--  2.0 unx     2129 b- defN 22-Oct-22 15:53 exojax/special/j0.py
--rw-rw-r--  2.0 unx      525 b- defN 23-Mar-15 18:44 exojax/special/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     9801 b- defN 23-Mar-15 18:44 exojax/special/__pycache__/_special.cpython-38.pyc
--rw-rw-r--  2.0 unx     1244 b- defN 23-Mar-15 18:44 exojax/special/__pycache__/erfcx.cpython-38.pyc
--rw-rw-r--  2.0 unx     1066 b- defN 23-Mar-15 18:44 exojax/special/__pycache__/expn.cpython-38.pyc
--rw-rw-r--  2.0 unx     4683 b- defN 23-Mar-15 18:44 exojax/special/__pycache__/faddeeva.cpython-38.pyc
--rw-rw-r--  2.0 unx     1507 b- defN 23-Mar-15 18:44 exojax/special/__pycache__/j0.cpython-38.pyc
--rw-rw-r--  2.0 unx       14 b- defN 22-Dec-07 21:18 exojax/test/__init__.py
--rw-rw-r--  2.0 unx     1666 b- defN 23-Mar-15 18:34 exojax/test/data.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Feb-06 22:31 exojax/test/emulate_broadpar.py
--rw-rw-r--  2.0 unx     2774 b- defN 23-Mar-15 18:34 exojax/test/emulate_mdb.py
+-rw-rw-r--  2.0 unx      525 b- defN 23-Jun-01 18:04 exojax/special/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     9801 b- defN 23-Jun-01 18:04 exojax/special/__pycache__/_special.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1244 b- defN 23-Jun-01 18:04 exojax/special/__pycache__/erfcx.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-01 18:04 exojax/special/__pycache__/expn.cpython-38.pyc
+-rw-rw-r--  2.0 unx     4683 b- defN 23-Jun-01 18:04 exojax/special/__pycache__/faddeeva.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1507 b- defN 23-Jun-01 18:04 exojax/special/__pycache__/j0.cpython-38.pyc
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-09 09:44 exojax/test/__init__.py
+-rw-rw-r--  2.0 unx     1666 b- defN 23-Jun-01 17:59 exojax/test/data.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-01 17:59 exojax/test/emulate_broadpar.py
+-rw-rw-r--  2.0 unx     2774 b- defN 23-Jun-01 17:59 exojax/test/emulate_mdb.py
 -rw-rw-r--  2.0 unx     1509 b- defN 23-Feb-04 11:33 exojax/test/emulate_mdb_current.py
--rw-rw-r--  2.0 unx     1843 b- defN 23-Mar-15 18:34 exojax/test/generate.py
--rw-rw-r--  2.0 unx     2591 b- defN 23-Mar-15 18:34 exojax/test/generate_mdb.py
--rw-rw-r--  2.0 unx     3278 b- defN 23-Mar-15 18:34 exojax/test/generate_methane_spectrum.py
--rw-rw-r--  2.0 unx     4139 b- defN 23-Mar-15 18:34 exojax/test/generate_rt.py
--rw-rw-r--  2.0 unx     4954 b- defN 23-Mar-15 18:34 exojax/test/generate_xs.py
--rw-rw-r--  2.0 unx      153 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     1572 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/data.cpython-38.pyc
--rw-rw-r--  2.0 unx     1142 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/emulate_broadpar.cpython-38.pyc
--rw-rw-r--  2.0 unx     2644 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/emulate_mdb.cpython-38.pyc
--rw-rw-r--  2.0 unx     1557 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/emulate_mdb_current.cpython-38.pyc
--rw-rw-r--  2.0 unx     1790 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/generate.cpython-38.pyc
--rw-rw-r--  2.0 unx     1855 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/generate_mdb.cpython-38.pyc
--rw-rw-r--  2.0 unx     2826 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/generate_methane_spectrum.cpython-38.pyc
--rw-rw-r--  2.0 unx     2901 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/generate_rt.cpython-38.pyc
--rw-rw-r--  2.0 unx     3817 b- defN 23-Mar-15 18:44 exojax/test/__pycache__/generate_xs.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1843 b- defN 23-Apr-09 09:45 exojax/test/generate.py
+-rw-rw-r--  2.0 unx     2591 b- defN 23-Apr-09 09:46 exojax/test/generate_mdb.py
+-rw-rw-r--  2.0 unx     3278 b- defN 23-Jun-01 17:59 exojax/test/generate_methane_spectrum.py
+-rw-rw-r--  2.0 unx     3736 b- defN 23-Apr-12 12:49 exojax/test/generate_methane_trans.py
+-rw-rw-r--  2.0 unx     4139 b- defN 23-Jun-01 17:59 exojax/test/generate_rt.py
+-rw-rw-r--  2.0 unx     4954 b- defN 23-Jun-01 17:59 exojax/test/generate_xs.py
+-rw-rw-r--  2.0 unx      153 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/data.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1142 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/emulate_broadpar.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2644 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/emulate_mdb.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1557 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/emulate_mdb_current.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1790 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/generate.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1855 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/generate_mdb.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2826 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/generate_methane_spectrum.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2934 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/generate_methane_trans.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2901 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/generate_rt.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3817 b- defN 23-Jun-01 18:04 exojax/test/__pycache__/generate_xs.cpython-38.pyc
 -rw-rw-r--  2.0 unx      176 b- defN 23-Feb-06 22:31 exojax/utils/__init__.py
 -rw-rw-r--  2.0 unx      973 b- defN 22-Oct-26 08:56 exojax/utils/afunc.py
 -rw-rw-r--  2.0 unx      943 b- defN 23-Mar-15 18:34 exojax/utils/astrofunc.py
 -rw-rw-r--  2.0 unx      650 b- defN 23-Feb-06 22:31 exojax/utils/chopstacks.py
--rw-rw-r--  2.0 unx     1574 b- defN 23-Mar-15 18:34 exojax/utils/constants.py
+-rw-rw-r--  2.0 unx     1574 b- defN 23-Jun-01 17:59 exojax/utils/constants.py
 -rw-rw-r--  2.0 unx      876 b- defN 22-Oct-15 09:05 exojax/utils/delta_velocity.py
 -rw-rw-r--  2.0 unx     1970 b- defN 23-Mar-15 08:00 exojax/utils/exofile.py
 -rw-rw-r--  2.0 unx      422 b- defN 22-May-01 08:50 exojax/utils/gpkernel.py
--rw-rw-r--  2.0 unx     5441 b- defN 23-Mar-15 18:34 exojax/utils/grids.py
+-rw-rw-r--  2.0 unx     5441 b- defN 23-Jun-01 17:59 exojax/utils/grids.py
 -rw-rw-r--  2.0 unx     5206 b- defN 23-Feb-06 22:31 exojax/utils/indexing.py
--rw-rw-r--  2.0 unx     1554 b- defN 23-Mar-15 18:34 exojax/utils/instfunc.py
+-rw-rw-r--  2.0 unx     1554 b- defN 23-Mar-19 10:35 exojax/utils/instfunc.py
 -rw-rw-r--  2.0 unx      902 b- defN 22-Dec-23 06:46 exojax/utils/isodata.py
 -rw-rw-r--  2.0 unx     3326 b- defN 23-Mar-15 18:34 exojax/utils/isotopes.py
--rw-rw-r--  2.0 unx     6145 b- defN 23-Mar-15 18:34 exojax/utils/molname.py
+-rw-rw-r--  2.0 unx      896 b- defN 23-May-20 11:55 exojax/utils/jaxstatus.py
+-rw-rw-r--  2.0 unx     2664 b- defN 23-May-20 11:42 exojax/utils/memuse.py
+-rw-rw-r--  2.0 unx     6145 b- defN 23-Mar-19 10:35 exojax/utils/molname.py
 -rw-rw-r--  2.0 unx      565 b- defN 23-Mar-15 18:34 exojax/utils/progbar.py
 -rw-rw-r--  2.0 unx     1772 b- defN 22-May-01 08:50 exojax/utils/recexomol.py
 -rw-rw-r--  2.0 unx     1599 b- defN 22-Oct-26 08:25 exojax/utils/url.py
 -rw-rw-r--  2.0 unx     4017 b- defN 22-Sep-05 20:45 exojax/utils/zsol.py
--rw-rw-r--  2.0 unx      338 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--  2.0 unx     1288 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/afunc.cpython-38.pyc
--rw-rw-r--  2.0 unx     1240 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/astrofunc.cpython-38.pyc
--rw-rw-r--  2.0 unx      861 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/chopstacks.cpython-38.pyc
--rw-rw-r--  2.0 unx     1028 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/constants.cpython-38.pyc
--rw-rw-r--  2.0 unx     1133 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/delta_velocity.cpython-38.pyc
--rw-rw-r--  2.0 unx     1984 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/exofile.cpython-38.pyc
--rw-rw-r--  2.0 unx      665 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/gpkernel.cpython-38.pyc
--rw-rw-r--  2.0 unx     5966 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/grids.cpython-38.pyc
--rw-rw-r--  2.0 unx     5100 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/indexing.cpython-38.pyc
--rw-rw-r--  2.0 unx     2010 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/instfunc.cpython-38.pyc
--rw-rw-r--  2.0 unx     1131 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/isodata.cpython-38.pyc
--rw-rw-r--  2.0 unx     3121 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/isotopes.cpython-38.pyc
--rw-rw-r--  2.0 unx     5633 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/molname.cpython-38.pyc
--rw-rw-r--  2.0 unx      714 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/progbar.cpython-38.pyc
--rw-rw-r--  2.0 unx     1993 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/recexomol.cpython-38.pyc
--rw-rw-r--  2.0 unx     2111 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/url.cpython-38.pyc
--rw-rw-r--  2.0 unx     3706 b- defN 23-Mar-15 18:44 exojax/utils/__pycache__/zsol.cpython-38.pyc
-275 files, 57213553 bytes uncompressed, 6761434 bytes compressed:  88.2%
+-rw-rw-r--  2.0 unx      338 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/afunc.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/astrofunc.cpython-38.pyc
+-rw-rw-r--  2.0 unx      861 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/chopstacks.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1028 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/constants.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/delta_velocity.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1984 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/exofile.cpython-38.pyc
+-rw-rw-r--  2.0 unx      665 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/gpkernel.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5966 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/grids.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5100 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/indexing.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2010 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/instfunc.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1131 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/isodata.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3121 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/isotopes.cpython-38.pyc
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/jaxstatus.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2339 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/memuse.cpython-38.pyc
+-rw-rw-r--  2.0 unx     5633 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/molname.cpython-38.pyc
+-rw-rw-r--  2.0 unx      714 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/progbar.cpython-38.pyc
+-rw-rw-r--  2.0 unx     1993 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/recexomol.cpython-38.pyc
+-rw-rw-r--  2.0 unx     2111 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/url.cpython-38.pyc
+-rw-rw-r--  2.0 unx     3706 b- defN 23-Jun-01 18:04 exojax/utils/__pycache__/zsol.cpython-38.pyc
+295 files, 57252779 bytes uncompressed, 6778336 bytes compressed:  88.2%
```

## zipnote «TEMP»/diffoscope_lxz4w28o_/tmpr47tyhsx_.zip

```diff
@@ -15,17 +15,29 @@
 
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
 Filename: exojax/__init__.py
 Comment: 
 
+Filename: exojax/data.py
+Comment: 
+
+Filename: exojax/emulate_broadpar.py
+Comment: 
+
 Filename: exojax/__pycache__/__init__.cpython-38.pyc
 Comment: 
 
+Filename: exojax/__pycache__/data.cpython-38.pyc
+Comment: 
+
+Filename: exojax/__pycache__/emulate_broadpar.cpython-38.pyc
+Comment: 
+
 Filename: exojax/atm/__init__.py
 Comment: 
 
 Filename: exojax/atm/amclouds.py
 Comment: 
 
 Filename: exojax/atm/atmprof.py
@@ -234,23 +246,29 @@
 
 Filename: exojax/plot/atmplot.py
 Comment: 
 
 Filename: exojax/plot/ditplot.py
 Comment: 
 
+Filename: exojax/plot/opaplot.py
+Comment: 
+
 Filename: exojax/plot/__pycache__/__init__.cpython-38.pyc
 Comment: 
 
 Filename: exojax/plot/__pycache__/atmplot.cpython-38.pyc
 Comment: 
 
 Filename: exojax/plot/__pycache__/ditplot.cpython-38.pyc
 Comment: 
 
+Filename: exojax/plot/__pycache__/opaplot.cpython-38.pyc
+Comment: 
+
 Filename: exojax/signal/__init__.py
 Comment: 
 
 Filename: exojax/signal/convolve.py
 Comment: 
 
 Filename: exojax/signal/ola.py
@@ -369,14 +387,17 @@
 
 Filename: exojax/spec/moldf.py
 Comment: 
 
 Filename: exojax/spec/molinfo.py
 Comment: 
 
+Filename: exojax/spec/nonair.py
+Comment: 
+
 Filename: exojax/spec/opacalc.py
 Comment: 
 
 Filename: exojax/spec/opachord.py
 Comment: 
 
 Filename: exojax/spec/opacity.py
@@ -384,14 +405,17 @@
 
 Filename: exojax/spec/opacitytools.py
 Comment: 
 
 Filename: exojax/spec/opacont.py
 Comment: 
 
+Filename: exojax/spec/opspec.py
+Comment: 
+
 Filename: exojax/spec/optgrid.py
 Comment: 
 
 Filename: exojax/spec/planck.py
 Comment: 
 
 Filename: exojax/spec/plg.py
@@ -402,14 +426,17 @@
 
 Filename: exojax/spec/presolar.py
 Comment: 
 
 Filename: exojax/spec/presolar_scanola.py
 Comment: 
 
+Filename: exojax/spec/qstate.py
+Comment: 
+
 Filename: exojax/spec/radis_test.py
 Comment: 
 
 Filename: exojax/spec/response.py
 Comment: 
 
 Filename: exojax/spec/rtcheck.py
@@ -429,14 +456,17 @@
 
 Filename: exojax/spec/setrt.py
 Comment: 
 
 Filename: exojax/spec/shapefilter.py
 Comment: 
 
+Filename: exojax/spec/specop.py
+Comment: 
+
 Filename: exojax/spec/spin_rotation.py
 Comment: 
 
 Filename: exojax/spec/tau1height.py
 Comment: 
 
 Filename: exojax/spec/unitconvert.py
@@ -546,14 +576,17 @@
 
 Filename: exojax/spec/__pycache__/moldf.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/molinfo.cpython-38.pyc
 Comment: 
 
+Filename: exojax/spec/__pycache__/nonair.cpython-38.pyc
+Comment: 
+
 Filename: exojax/spec/__pycache__/opacalc.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/opachord.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/opacity.cpython-38.pyc
@@ -561,14 +594,17 @@
 
 Filename: exojax/spec/__pycache__/opacitytools.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/opacont.cpython-38.pyc
 Comment: 
 
+Filename: exojax/spec/__pycache__/opspec.cpython-38.pyc
+Comment: 
+
 Filename: exojax/spec/__pycache__/optgrid.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/planck.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/plg.cpython-38.pyc
@@ -579,14 +615,17 @@
 
 Filename: exojax/spec/__pycache__/presolar.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/presolar_scanola.cpython-38.pyc
 Comment: 
 
+Filename: exojax/spec/__pycache__/qstate.cpython-38.pyc
+Comment: 
+
 Filename: exojax/spec/__pycache__/radis_test.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/response.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/rtcheck.cpython-38.pyc
@@ -606,14 +645,17 @@
 
 Filename: exojax/spec/__pycache__/setrt.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/shapefilter.cpython-38.pyc
 Comment: 
 
+Filename: exojax/spec/__pycache__/specop.cpython-38.pyc
+Comment: 
+
 Filename: exojax/spec/__pycache__/spin_rotation.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/tau1height.cpython-38.pyc
 Comment: 
 
 Filename: exojax/spec/__pycache__/unitconvert.cpython-38.pyc
@@ -675,14 +717,17 @@
 
 Filename: exojax/test/generate_mdb.py
 Comment: 
 
 Filename: exojax/test/generate_methane_spectrum.py
 Comment: 
 
+Filename: exojax/test/generate_methane_trans.py
+Comment: 
+
 Filename: exojax/test/generate_rt.py
 Comment: 
 
 Filename: exojax/test/generate_xs.py
 Comment: 
 
 Filename: exojax/test/__pycache__/__init__.cpython-38.pyc
@@ -705,14 +750,17 @@
 
 Filename: exojax/test/__pycache__/generate_mdb.cpython-38.pyc
 Comment: 
 
 Filename: exojax/test/__pycache__/generate_methane_spectrum.cpython-38.pyc
 Comment: 
 
+Filename: exojax/test/__pycache__/generate_methane_trans.cpython-38.pyc
+Comment: 
+
 Filename: exojax/test/__pycache__/generate_rt.cpython-38.pyc
 Comment: 
 
 Filename: exojax/test/__pycache__/generate_xs.cpython-38.pyc
 Comment: 
 
 Filename: exojax/utils/__init__.py
@@ -750,14 +798,20 @@
 
 Filename: exojax/utils/isodata.py
 Comment: 
 
 Filename: exojax/utils/isotopes.py
 Comment: 
 
+Filename: exojax/utils/jaxstatus.py
+Comment: 
+
+Filename: exojax/utils/memuse.py
+Comment: 
+
 Filename: exojax/utils/molname.py
 Comment: 
 
 Filename: exojax/utils/progbar.py
 Comment: 
 
 Filename: exojax/utils/recexomol.py
@@ -804,14 +858,20 @@
 
 Filename: exojax/utils/__pycache__/isodata.cpython-38.pyc
 Comment: 
 
 Filename: exojax/utils/__pycache__/isotopes.cpython-38.pyc
 Comment: 
 
+Filename: exojax/utils/__pycache__/jaxstatus.cpython-38.pyc
+Comment: 
+
+Filename: exojax/utils/__pycache__/memuse.cpython-38.pyc
+Comment: 
+
 Filename: exojax/utils/__pycache__/molname.cpython-38.pyc
 Comment: 
 
 Filename: exojax/utils/__pycache__/progbar.cpython-38.pyc
 Comment: 
 
 Filename: exojax/utils/__pycache__/recexomol.cpython-38.pyc
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExoJAX
-Version: 1.3
+Version: 1.3.1
 Summary: Auto-differentiable line-by-line spectral modeling of exoplanets/brown dwarfs using JAX.
 Home-page: http://secondearths.sakura.ne.jp/exojax/
 Author: Hajime Kawahara and collaborators
 Author-email: divrot@gmail.com
 Maintainer: Hajime Kawahara and collaborators
 Maintainer-email: divrot@gmail.com
 License: MIT
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ExoJAX Version: 1.3 Summary: Auto-differentiable
+Metadata-Version: 2.1 Name: ExoJAX Version: 1.3.1 Summary: Auto-differentiable
 line-by-line spectral modeling of exoplanets/brown dwarfs using JAX. Home-page:
 http://secondearths.sakura.ne.jp/exojax/ Author: Hajime Kawahara and
 collaborators Author-email: divrot@gmail.com Maintainer: Hajime Kawahara and
 collaborators Maintainer-email: divrot@gmail.com License: MIT Platform: UNKNOWN
 Classifier: Programming Language :: Python Description-Content-Type: text/
 markdown License-File: LICENSE License-File: LICENSES_bundled.txt # ExoJAX [!
 [License](https://img.shields.io/github/license/HajimeKawahara/exojax)](https:/
```

## EGG-INFO/SOURCES.txt

```diff
@@ -137,19 +137,17 @@
 tests/.database/gf2600.all
 tests/.database/vald2600.gz
 tests/.database/vald2600.hdf5
 tests/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/CO/05_HITEMP_SAMPLE.hdf5
 tests/CO/05_HITEMP_SAMPLE.par
 tests/CO/12C-16O/SAMPLE/12C-16O__H2.broad
 tests/CO/12C-16O/SAMPLE/12C-16O__He.broad
 tests/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.def
 tests/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.pf
@@ -165,15 +163,14 @@
 tests/benchmark/a100/lpf.dat
 tests/benchmark/fig/read_dat.py
 tests/benchmark/fig/data/each.dat
 tests/benchmark/fig/data/each2.dat
 tests/benchmark/fig/data/gpu.dat
 tests/benchmark/fig/data/gpu2.dat
 tests/endtoend/.database/CO-05_HITEMP2019.hdf5
-tests/endtoend/.database/CO.hdf5
 tests/endtoend/.database/H2-H2_2011.cia
 tests/endtoend/.database/H2-He_2011.cia
 tests/endtoend/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/endtoend/.database/HiroyukiIshikawa.4214450.gz
 tests/endtoend/.database/HiroyukiIshikawa.4214450.hdf5
 tests/endtoend/.database/gf2600.all
 tests/endtoend/.database/gj699_coadded_cr2.dat
@@ -225,19 +222,17 @@
 tests/endtoend/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/endtoend/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/endtoend/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/endtoend/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/endtoend/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/endtoend/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/endtoend/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/endtoend/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/endtoend/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/endtoend/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -280,14 +275,15 @@
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/endtoend/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/endtoend/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/endtoend/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/endtoend/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/endtoend/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/endtoend/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/endtoend/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -362,15 +358,14 @@
 tests/endtoend/jaxopt/.database/CO/12C-16O/Li2015/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
 tests/endtoend/jaxopt/.database/CO/12C-16O/Li2015/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/endtoend/jaxopt/.database/CO/12C-16O/Li2015/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/endtoend/metals/Kurucz_linelist_test.py
 tests/endtoend/metals/VALD_MODIT_test.py
 tests/endtoend/metals/opacity_Fe_test.py
 tests/endtoend/metals/.database/CO-05_HITEMP2019.hdf5
-tests/endtoend/metals/.database/CO.hdf5
 tests/endtoend/metals/.database/H2-H2_2011.cia
 tests/endtoend/metals/.database/H2-He_2011.cia
 tests/endtoend/metals/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/endtoend/metals/.database/HiroyukiIshikawa.4214450.gz
 tests/endtoend/metals/.database/HiroyukiIshikawa.4214450.hdf5
 tests/endtoend/metals/.database/gf2600.all
 tests/endtoend/metals/.database/gj699_coadded_cr2.dat
@@ -422,19 +417,17 @@
 tests/endtoend/metals/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/endtoend/metals/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/endtoend/metals/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/endtoend/metals/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/endtoend/metals/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/endtoend/metals/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/endtoend/metals/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/endtoend/metals/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/endtoend/metals/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/endtoend/metals/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -477,14 +470,15 @@
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/endtoend/metals/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/endtoend/metals/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/endtoend/metals/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/endtoend/metals/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/endtoend/metals/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/endtoend/metals/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/endtoend/metals/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -549,15 +543,14 @@
 tests/endtoend/reverse/reverse_premodit_blackjax.py
 tests/endtoend/reverse/spectrum.png
 tests/endtoend/reverse/spectrum.txt
 tests/endtoend/reverse/spectrum_ch4.txt
 tests/endtoend/reverse/spectrum_ch4_new.txt
 tests/endtoend/reverse/spectrum_co.txt
 tests/endtoend/reverse/.database/CO-05_HITEMP2019.hdf5
-tests/endtoend/reverse/.database/CO.hdf5
 tests/endtoend/reverse/.database/H2-H2_2011.cia
 tests/endtoend/reverse/.database/H2-He_2011.cia
 tests/endtoend/reverse/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/endtoend/reverse/.database/HiroyukiIshikawa.4214450.gz
 tests/endtoend/reverse/.database/HiroyukiIshikawa.4214450.hdf5
 tests/endtoend/reverse/.database/gf2600.all
 tests/endtoend/reverse/.database/gj699_coadded_cr2.dat
@@ -609,19 +602,17 @@
 tests/endtoend/reverse/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/endtoend/reverse/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/endtoend/reverse/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/endtoend/reverse/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/endtoend/reverse/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/endtoend/reverse/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/endtoend/reverse/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/endtoend/reverse/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/endtoend/reverse/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/endtoend/reverse/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -664,14 +655,15 @@
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/endtoend/reverse/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/endtoend/reverse/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/endtoend/reverse/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/endtoend/reverse/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/endtoend/reverse/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/endtoend/reverse/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/endtoend/reverse/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -775,22 +767,29 @@
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__He.broad
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.def
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.pf
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.bz2
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.hdf5
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.bz2
 tests/integration/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.hdf5
+tests/integration/api/CO-05_HITEMP2019.hdf5
+tests/integration/api/CO.hdf5
+tests/integration/api/test_api.py~
+tests/integration/broadening/braodpar_grid.png
+tests/integration/broadening/broadpar_grid.png
+tests/integration/broadening/.database/H2O/H2O-01_04150-04500_HITEMP2010.hdf5
+tests/integration/broadening/.temp/H2O/H2O-01_04150-04500_HITEMP2010.hdf5
 tests/integration/comparison/.database/CH4/12C-1H4/YT10to10/12C-1H4__H2.broad
 tests/integration/comparison/.database/CH4/12C-1H4/YT10to10/12C-1H4__He.broad
 tests/integration/comparison/.database/CH4/12C-1H4/YT10to10/12C-1H4__YT10to10.def
 tests/integration/comparison/.database/CH4/12C-1H4/YT10to10/12C-1H4__YT10to10.pf
 tests/integration/comparison/.database/CH4/12C-1H4/YT10to10/12C-1H4__YT10to10.states.bz2
+tests/integration/comparison/nonair/CO.hdf5
 tests/integration/comparison/premodit/comp_lsd_test.py
 tests/integration/comparison/premodit/.database/CO-05_HITEMP2019.hdf5
-tests/integration/comparison/premodit/.database/CO.hdf5
 tests/integration/comparison/premodit/.database/H2-H2_2011.cia
 tests/integration/comparison/premodit/.database/H2-He_2011.cia
 tests/integration/comparison/premodit/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/integration/comparison/premodit/.database/HiroyukiIshikawa.4214450.gz
 tests/integration/comparison/premodit/.database/HiroyukiIshikawa.4214450.hdf5
 tests/integration/comparison/premodit/.database/gf2600.all
 tests/integration/comparison/premodit/.database/gj699_coadded_cr2.dat
@@ -842,19 +841,17 @@
 tests/integration/comparison/premodit/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/integration/comparison/premodit/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/integration/comparison/premodit/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/integration/comparison/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/integration/comparison/premodit/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/integration/comparison/premodit/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/integration/comparison/premodit/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/integration/comparison/premodit/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/integration/comparison/premodit/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/integration/comparison/premodit/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -897,14 +894,15 @@
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/integration/comparison/premodit/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/integration/comparison/premodit/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/integration/comparison/premodit/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/integration/comparison/premodit/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/integration/comparison/premodit/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -967,16 +965,21 @@
 tests/integration/exomol_check/NaH/23Na-1H/Rivlin/23Na-1H__Rivlin.trans.hdf5
 tests/integration/modit_scanfft/modit_scanfft_test.py
 tests/integration/modit_scanfft/modit_scanfft_test.py~
 tests/integration/moldb/05_HITEMP2019.par~
 tests/integration/moldb/05_HITEMP_SAMPLE.hdf5
 tests/integration/moldb/CO-05_HITEMP2019.hdf5
 tests/integration/moldb/CO.hdf5
+tests/integration/moldb/comp_nonair_1.png
+tests/integration/moldb/comp_nonair_2.png
 tests/integration/moldb/comparison_api.py
 tests/integration/moldb/comparison_api_xs.py
+tests/integration/moldb/comph2_1.png
+tests/integration/moldb/comph2_2.png
+tests/integration/moldb/hitemp_co_noair_h2.png
 tests/integration/moldb/mdbexomol_test.py
 tests/integration/moldb/mdbhitemp_test.py
 tests/integration/moldb/mdbhitemp_test.py~
 tests/integration/moldb/mdbhitran_test.py
 tests/integration/moldb/quantum_states_filter_exomol.py
 tests/integration/moldb/quantum_states_filter_hitemp.py
 tests/integration/moldb/quantum_states_filter_hitran_co.py
@@ -1013,20 +1016,29 @@
 tests/integration/opacalc/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.bz2
 tests/integration/opacalc/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.hdf5
 tests/integration/opacalc/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.bz2
 tests/integration/opacalc/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.hdf5
 tests/integration/premodit/CO-05_HITEMP2019.hdf5
 tests/integration/premodit/checkindex.py
 tests/integration/premodit/comp_mock_api.py
+tests/integration/premodit/fftpower2.py~
 tests/integration/premodit/line_strength_comparison_exomol.py
 tests/integration/premodit/line_strength_comparison_exomol_water.py
 tests/integration/premodit/line_strength_comparison_hitemp.py
 tests/integration/premodit/premodit0.png
 tests/integration/premodit/temp_hitemp.txt
 tests/integration/premodit/xsv_modit.txt
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__He.broad
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
+tests/integration/premodit/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__H2.broad
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__He.broad
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.def
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.pf
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.states.bz2
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.states.bz2.yaml
 tests/integration/premodit/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.states.hdf5
@@ -1049,15 +1061,14 @@
 tests/integration/premodit/oldpng/ic0.2_1200K.png
 tests/integration/premodit/oldpng/ic0.2_700K.png
 tests/integration/premodit/oldpng/ic0.3.png
 tests/integration/premodit/oldpng/ic0.3_1200K.png
 tests/integration/premodit/oldpng/ic0.3_700K.png
 tests/manual_check/readme_sample.py
 tests/manual_check/.database/CO-05_HITEMP2019.hdf5
-tests/manual_check/.database/CO.hdf5
 tests/manual_check/.database/H2-H2_2011.cia
 tests/manual_check/.database/H2-He_2011.cia
 tests/manual_check/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/manual_check/.database/HiroyukiIshikawa.4214450.gz
 tests/manual_check/.database/HiroyukiIshikawa.4214450.hdf5
 tests/manual_check/.database/gf2600.all
 tests/manual_check/.database/gj699_coadded_cr2.dat
@@ -1109,19 +1120,17 @@
 tests/manual_check/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/manual_check/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/manual_check/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/manual_check/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/manual_check/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/manual_check/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/manual_check/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/manual_check/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/manual_check/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/manual_check/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -1164,14 +1173,15 @@
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/manual_check/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/manual_check/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/manual_check/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/manual_check/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/manual_check/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/manual_check/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/manual_check/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -1213,15 +1223,14 @@
 tests/manual_check/.database/VO/51V-16O/VOMYT/51V-16O__VOMYT.states.bz2
 tests/manual_check/.database/VO/51V-16O/VOMYT/51V-16O__VOMYT.states.bz2.yaml
 tests/manual_check/.database/VO/51V-16O/VOMYT/51V-16O__VOMYT__05000-10000.trans.bz2
 tests/manual_check/.database/VO/51V-16O/VOMYT/51V-16O__VOMYT__05000-10000.trans.bz2.yaml
 tests/manual_check/auto/autort.py
 tests/manual_check/auto/autoxs.py
 tests/manual_check/auto/.database/CO-05_HITEMP2019.hdf5
-tests/manual_check/auto/.database/CO.hdf5
 tests/manual_check/auto/.database/H2-H2_2011.cia
 tests/manual_check/auto/.database/H2-He_2011.cia
 tests/manual_check/auto/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/manual_check/auto/.database/HiroyukiIshikawa.4214450.gz
 tests/manual_check/auto/.database/HiroyukiIshikawa.4214450.hdf5
 tests/manual_check/auto/.database/gf2600.all
 tests/manual_check/auto/.database/gj699_coadded_cr2.dat
@@ -1273,19 +1282,17 @@
 tests/manual_check/auto/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/manual_check/auto/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/manual_check/auto/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/manual_check/auto/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/manual_check/auto/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/manual_check/auto/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/manual_check/auto/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/manual_check/auto/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/manual_check/auto/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/manual_check/auto/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -1328,14 +1335,15 @@
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/manual_check/auto/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/manual_check/auto/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/manual_check/auto/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/manual_check/auto/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/manual_check/auto/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/manual_check/auto/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/manual_check/auto/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -1382,15 +1390,14 @@
 tests/manual_check/comparison/comparison_getE.py
 tests/manual_check/comparison/comparison_modit.pdf
 tests/manual_check/comparison/comparison_modit.png
 tests/manual_check/comparison/dit_hitran_CO.py
 tests/manual_check/comparison/modit_comparison.py
 tests/manual_check/comparison/modit_hitran_CO.py
 tests/manual_check/comparison/.database/CO-05_HITEMP2019.hdf5
-tests/manual_check/comparison/.database/CO.hdf5
 tests/manual_check/comparison/.database/H2-H2_2011.cia
 tests/manual_check/comparison/.database/H2-He_2011.cia
 tests/manual_check/comparison/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/manual_check/comparison/.database/HiroyukiIshikawa.4214450.gz
 tests/manual_check/comparison/.database/HiroyukiIshikawa.4214450.hdf5
 tests/manual_check/comparison/.database/gf2600.all
 tests/manual_check/comparison/.database/gj699_coadded_cr2.dat
@@ -1442,19 +1449,17 @@
 tests/manual_check/comparison/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/manual_check/comparison/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/manual_check/comparison/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/manual_check/comparison/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/manual_check/comparison/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/manual_check/comparison/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/manual_check/comparison/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/manual_check/comparison/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/manual_check/comparison/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/manual_check/comparison/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -1497,14 +1502,15 @@
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/manual_check/comparison/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/manual_check/comparison/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/manual_check/comparison/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/manual_check/comparison/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/manual_check/comparison/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/manual_check/comparison/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/manual_check/comparison/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -1549,15 +1555,14 @@
 tests/manual_check/comparison/.database/VO/51V-16O/VOMYT/51V-16O__VOMYT__05000-10000.trans.bz2.yaml
 tests/manual_check/comparison/hi_dynamic_range/README.md
 tests/manual_check/comparison/hi_dynamic_range/errCO_DIT.py
 tests/manual_check/comparison/hi_dynamic_range/errCO_MODIT.py
 tests/manual_check/comparison/hi_dynamic_range/errCO_REDIT.py
 tests/manual_check/xs/Ttyp_demo.py
 tests/manual_check/xs/.database/CO-05_HITEMP2019.hdf5
-tests/manual_check/xs/.database/CO.hdf5
 tests/manual_check/xs/.database/H2-H2_2011.cia
 tests/manual_check/xs/.database/H2-He_2011.cia
 tests/manual_check/xs/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/manual_check/xs/.database/HiroyukiIshikawa.4214450.gz
 tests/manual_check/xs/.database/HiroyukiIshikawa.4214450.hdf5
 tests/manual_check/xs/.database/gf2600.all
 tests/manual_check/xs/.database/gj699_coadded_cr2.dat
@@ -1609,19 +1614,17 @@
 tests/manual_check/xs/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/manual_check/xs/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/manual_check/xs/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/manual_check/xs/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/manual_check/xs/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/manual_check/xs/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/manual_check/xs/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/manual_check/xs/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/manual_check/xs/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/manual_check/xs/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -1664,14 +1667,15 @@
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/manual_check/xs/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/manual_check/xs/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/manual_check/xs/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/manual_check/xs/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/manual_check/xs/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/manual_check/xs/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/manual_check/xs/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -1722,15 +1726,14 @@
 tests/plg/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.states.bz2.hdf5
 tests/plg/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL.states.bz2.yaml
 tests/plg/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06400-06500.trans.bz2
 tests/unittests/premodit0.png
 tests/unittests/premodit1.png
 tests/unittests/premodit2.png
 tests/unittests/.database/CO-05_HITEMP2019.hdf5
-tests/unittests/.database/CO.hdf5
 tests/unittests/.database/H2-H2_2011.cia
 tests/unittests/.database/H2-He_2011.cia
 tests/unittests/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/unittests/.database/HiroyukiIshikawa.4214450.gz
 tests/unittests/.database/HiroyukiIshikawa.4214450.hdf5
 tests/unittests/.database/gf2600.all
 tests/unittests/.database/gj699_coadded_cr2.dat
@@ -1782,19 +1785,17 @@
 tests/unittests/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/unittests/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/unittests/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/unittests/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/unittests/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/unittests/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/unittests/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/unittests/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/unittests/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/unittests/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -1837,14 +1838,15 @@
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/unittests/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/unittests/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/unittests/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/unittests/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/unittests/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/unittests/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/unittests/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -1902,15 +1904,14 @@
 tests/unittests/atom/molmass_test.py
 tests/unittests/dynamics/test_getE.py
 tests/unittests/install/func.py
 tests/unittests/readme_sample/readme_sample_test.py
 tests/unittests/signal/ola_test.py
 tests/unittests/signal/optimal_block_size.png
 tests/unittests/spec/.database/CO-05_HITEMP2019.hdf5
-tests/unittests/spec/.database/CO.hdf5
 tests/unittests/spec/.database/H2-H2_2011.cia
 tests/unittests/spec/.database/H2-He_2011.cia
 tests/unittests/spec/.database/HiroyukiIshikawa.4203812_test0724.ip
 tests/unittests/spec/.database/HiroyukiIshikawa.4214450.gz
 tests/unittests/spec/.database/HiroyukiIshikawa.4214450.hdf5
 tests/unittests/spec/.database/gf2600.all
 tests/unittests/spec/.database/gj699_coadded_cr2.dat
@@ -1962,19 +1963,17 @@
 tests/unittests/spec/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.bz2
 tests/unittests/spec/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10.states.hdf5
 tests/unittests/spec/.database/CH4/12C-1H4/YT34to10/12C-1H4__YT34to10__06100-06200.trans.bz2
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__H2.broad
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__He.broad
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.def
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.pf
-tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2
-tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.bz2.yaml
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.states.hdf5
-tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans
+tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.bz2
 tests/unittests/spec/.database/CO/12C-16O/Li2015/12C-16O__Li2015.trans.hdf5
 tests/unittests/spec/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.def
 tests/unittests/spec/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.pf
 tests/unittests/spec/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2
 tests/unittests/spec/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.states.bz2.yaml
 tests/unittests/spec/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2
 tests/unittests/spec/.database/CrH/52Cr-1H/MoLLIST/52Cr-1H__MoLLIST.trans.bz2.yaml
@@ -2017,14 +2016,15 @@
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06600-06700.trans.bz2
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06700-06800.trans.bz2.yaml
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06800-06900.trans.bz2.yaml
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.bz2.yaml
+tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__06900-07000.trans.hdf5
 tests/unittests/spec/.database/H2O/1H2-16O/POKAZATEL/1H2-16O__POKAZATEL__09600-09700.trans.bz2
 tests/unittests/spec/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__H2.broad
 tests/unittests/spec/.database/H2O/1H2-16O/PPOKAZATEL/1H2-16O__He.broad
 tests/unittests/spec/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__H2.broad
 tests/unittests/spec/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.def
 tests/unittests/spec/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.pf
 tests/unittests/spec/.database/HCN/1H-12C-14N/Harris/1H-12C-14N__Harris.states.bz2
@@ -2110,14 +2110,15 @@
 tests/unittests/spec/modit/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.def
 tests/unittests/spec/modit/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.pf
 tests/unittests/spec/modit/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.bz2
 tests/unittests/spec/modit/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.hdf5
 tests/unittests/spec/modit/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.bz2
 tests/unittests/spec/modit/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.hdf5
 tests/unittests/spec/opacitytools/pressure_at_given_opacity_test.py
+tests/unittests/spec/premodit/broadpar_grid.png
 tests/unittests/spec/premodit/lbd_test.py
 tests/unittests/spec/premodit/lbderror_test.py
 tests/unittests/spec/premodit/memory.prof
 tests/unittests/spec/premodit/optgrid_test.py
 tests/unittests/spec/premodit/premodit0.png
 tests/unittests/spec/premodit/premodit1.png
 tests/unittests/spec/premodit/premodit2.png
@@ -2168,8 +2169,18 @@
 tests/unittests/utils/chopstacks_test.py~
 tests/unittests/utils/grids_test.py
 tests/unittests/utils/indexing_test.py
 tests/unittests/utils/instfunc_test.py
 tests/unittests/utils/isotopes_test.py
 tests/unittests/utils/mnlist_test.py
 tests/unittests/utils/molname_test.py
-tests/unittests/utils/recexomol_test.py
+tests/unittests/utils/recexomol_test.py
+tests/unittests/utils/CO/05_HITEMP_SAMPLE.hdf5
+tests/unittests/utils/CO/05_HITEMP_SAMPLE.par
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__H2.broad
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__He.broad
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.def
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.pf
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.bz2
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.states.hdf5
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.bz2
+tests/unittests/utils/CO/12C-16O/SAMPLE/12C-16O__SAMPLE.trans.hdf5
```

## exojax/__pycache__/__init__.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Apr 30 23:50:13 2022 UTC, .py size: 298 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 35cb 6d62 2a01 0000  U.......5.mb*...
+00000000: 550d 0d0a 0000 0000 f75d 7864 2a01 0000  U........]xd*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 2000 0000 6700  .....@...s ...g.
 00000030: 5a00 6400 5a01 6401 5a02 6402 5a03 6403  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6404 5a05 6405 5a06 6406 5300 2907  Z.d.Z.d.Z.d.S.).
 00000050: 7a05 312e 302e 307a 2868 7474 703a 2f2f  z.1.0.0z(http://
 00000060: 7365 636f 6e64 6561 7274 6873 2e73 616b  secondearths.sak
 00000070: 7572 612e 6e65 2e6a 702f 6578 6f6a 6178  ura.ne.jp/exojax
```

## exojax/atm/__pycache__/atmprof.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 2719 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 9f0a 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 9f0a 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a06 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6405 8400 5a07 6406 6407 8400 5a08 6408  d...Z.d.d...Z.d.
 00000060: 6409 8400 5a09 6411 640b 640c 8401 5a0a  d...Z.d.d.d...Z.
 00000070: 640d 640e 8400 5a0b 640f 6410 8400 5a0c  d.d...Z.d.d...Z.
```

## exojax/spec/layeropacity.py

```diff
@@ -1,113 +1,115 @@
-"""compute opacity difference in atmospheric layers
+""" compute opacity difference in atmospheric layers
 
 """
 
 from jax import jit, vmap
 import jax.numpy as jnp
 from exojax.spec.hitrancia import interp_logacia_matrix
 from exojax.spec.hminus import log_hminus_continuum
 from exojax.atm.idealgas import number_density
 from exojax.utils.constants import logkB, logm_ucgs
 from exojax.utils.constants import opfac
 from exojax.spec.dtau_mmwl import dtauM_mmwl
 
 
-def layer_optical_depth(dParr, xsm, MR, mass, g):
+def layer_optical_depth(dParr, xsmatrix, mixing_ratio, mass, gravity):
     """dtau of the molecular cross section.
 
     Note:
-       opfac=bar_cgs/(m_u (g)). m_u: atomic mass unit. It can be obtained by fac=1.e3/m_u, where m_u = scipy.constants.m_u.
+        opfac=bar_cgs/(m_u (g)). m_u: atomic mass unit. It can be obtained by fac=1.e3/m_u, where m_u = scipy.constants.m_u.
 
     Args:
-       dParr: delta pressure profile (bar) [N_layer]
-       xsm: cross section matrix (cm2) [N_layer, N_nus]
-       MR: volume mixing ratio (VMR) or mass mixing ratio (MMR) [N_layer]
-       mass: mean molecular weight for VMR or molecular mass for MMR
-       g: gravity (cm/s2)
+        dParr: delta pressure profile (bar) [N_layer]
+        xsmatrix: cross section matrix (cm2) [N_layer, N_nus]
+        mixing_ratio: volume mixing ratio (VMR) or mass mixing ratio (MMR) [N_layer]
+        mass: mean molecular weight for VMR or molecular mass for MMR
+        gravity: gravity (cm/s2)
 
     Returns:
-       optical depth matrix [N_layer, N_nus]
+        2D array: optical depth matrix, dtau  [N_layer, N_nus]
     """
 
-    return opfac * xsm * dParr[:, None] * MR[:, None] / (mass * g)
+    return opfac * xsmatrix * dParr[:, None] * mixing_ratio[:, None] / (
+        mass * gravity)
 
 
-def layer_optical_depth_CIA(nus, Tarr, Parr, dParr, vmr1, vmr2, mmw, g, nucia, tcia, logac):
+def layer_optical_depth_CIA(nu_grid, temperature, pressure, dParr, vmr1, vmr2,
+                            mmw, g, nucia, tcia, logac):
     """dtau of the CIA continuum. Not used in art.
 
     Args:
-       nus: wavenumber matrix (cm-1)
-       Tarr: temperature array (K)
-       Parr: temperature array (bar)
-       dParr: delta temperature array (bar)
-       vmr1: volume mixing ratio (VMR) for molecules 1 [N_layer]
-       vmr2: volume mixing ratio (VMR) for molecules 2 [N_layer]
-       mmw: mean molecular weight of atmosphere
-       g: gravity (cm2/s)
-       nucia: wavenumber array for CIA
-       tcia: temperature array for CIA
-       logac: log10(absorption coefficient of CIA)
+        nu_grid: wavenumber matrix (cm-1)
+        temperature: temperature array (K)
+        pressure: pressure array (bar)
+        dParr: delta temperature array (bar)
+        vmr1: volume mixing ratio (VMR) for molecules 1 [N_layer]
+        vmr2: volume mixing ratio (VMR) for molecules 2 [N_layer]
+        mmw: mean molecular weight of atmosphere
+        g: gravity (cm2/s)
+        nucia: wavenumber array for CIA
+        tcia: temperature array for CIA
+        logac: log10(absorption coefficient of CIA)
 
     Returns:
-       optical depth matrix  [N_layer, N_nus]
+        2D array: optical depth matrix, dtau  [N_layer, N_nus]
     """
-    narr = number_density(Parr, Tarr)
+    narr = number_density(pressure, temperature)
     lognarr1 = jnp.log10(vmr1 * narr)  # log number density
     lognarr2 = jnp.log10(vmr2 * narr)  # log number density
     logg = jnp.log10(g)
-    ddParr = dParr / Parr
-    dtauc = (10**(interp_logacia_matrix(Tarr, nus, nucia, tcia, logac) +
-                  lognarr1[:, None] + lognarr2[:, None] + logkB - logg -
-                  logm_ucgs) * Tarr[:, None] / mmw * ddParr[:, None])
+    ddParr = dParr / pressure
+    dtauc = (
+        10**(interp_logacia_matrix(temperature, nu_grid, nucia, tcia, logac) +
+             lognarr1[:, None] + lognarr2[:, None] + logkB - logg - logm_ucgs)
+        * temperature[:, None] / mmw * ddParr[:, None])
 
     return dtauc
 
 
-def layer_optical_depth_VALD(dParr, xsm, VMR, mmw, g):
+def layer_optical_depth_VALD(dParr, xsm, VMR, mean_molecular_weight, gravity):
     """dtau of the atomic (+ionic) cross section from VALD.
 
     Args:
-       dParr: delta pressure profile (bar) [N_layer]
-       xsm: cross section matrix (cm2) [N_species x N_layer x N_wav]
-       VMR: volume mixing ratio [N_species x N_layer]
-       mmw: mean molecular weight [N_layer]
-       g: gravity (cm/s2)
+        dParr: delta pressure profile (bar) [N_layer]
+        xsm: cross section matrix (cm2) [N_species x N_layer x N_wav]
+        VMR: volume mixing ratio [N_species x N_layer]
+        mean_molecular_weight: mean molecular weight [N_layer]
+        gravity: gravity (cm/s2)
 
     Returns:
-        dtau: optical depth matrix [N_layer x N_nus]
+        2D array: optical depth matrix, dtau  [N_layer, N_nus]
     """
     dtauS = jit(vmap(dtauM_mmwl, (None, 0, 0, None, None)))( \
-                            dParr, xsm, VMR, mmw, g)
+                            dParr, xsm, VMR, mean_molecular_weight, gravity)
     dtau = jnp.abs(jnp.sum(dtauS, axis=0))
     return dtau
 
 
-def layer_optical_depth_Hminus(nus, Tarr, Parr, dParr, vmre, vmrh, mmw, g):
+def layer_optical_depth_Hminus(nu_grid, temperature, Parr, dParr, vmre, vmrh,
+                               mmw, g):
     """dtau of the H- continuum.
 
     Args:
-       nus: wavenumber matrix (cm-1)
-       Tarr: temperature array (K)
-       Parr: temperature array (bar)
-       dParr: delta temperature array (bar)
-       vmre: volume mixing ratio (VMR) for e- [N_layer]
-       vmrH: volume mixing ratio (VMR) for H atoms [N_layer]
-       mmw: mean molecular weight of atmosphere
-       g: gravity (cm2/s)
+        nu_grid: wavenumber matrix (cm-1)
+        Tarr: temperature array (K)
+        Parr: temperature array (bar)
+        dParr: delta temperature array (bar)
+        vmre: volume mixing ratio (VMR) for e- [N_layer]
+        vmrH: volume mixing ratio (VMR) for H atoms [N_layer]
+        mmw: mean molecular weight of atmosphere
+        g: gravity (cm2/s)
 
     Returns:
-       optical depth matrix  [N_layer, N_nus]
+        optical depth matrix  [N_layer, N_nus]
     """
-    narr = number_density(Parr, Tarr)
-    #       number_density_e: number density for e- [N_layer]
-    #       number_density_h: number density for H atoms [N_layer]
-    number_density_e = vmre * narr
-    number_density_h = vmrh * narr
+    narr = number_density(Parr, temperature)
+    number_density_e = vmre * narr  # number density for e- [N_layer]
+    number_density_h = vmrh * narr  # number density for H atoms [N_layer]
     logg = jnp.log10(g)
     ddParr = dParr / Parr
-    logabc = (log_hminus_continuum(nus, Tarr, number_density_e,
+    logabc = (log_hminus_continuum(nu_grid, temperature, number_density_e,
                                    number_density_h))
     dtauh = 10**(logabc + logkB - logg -
-                 logm_ucgs) * Tarr[:, None] / mmw * ddParr[:, None]
+                 logm_ucgs) * temperature[:, None] / mmw * ddParr[:, None]
 
     return dtauh
```

## exojax/spec/opachord.py

```diff
@@ -1,39 +1,44 @@
 import jax.numpy as jnp
 import numpy as np
 from jax import jit
 
 
 @jit
-def chord_geometric_matrix(height, radius):
+def chord_geometric_matrix(height, radius_lower):
     """compute chord geometric matrix
 
     Args:
         height (1D array): (normalized) height of the layers from top atmosphere, Nlayer
-        radius (1D array): (normalized) radius of the layers from top atmosphere, Nlayer
+        radius_lower (1D array): (normalized) radius at the lower boundary from top to bottom (R0), (Nlayer)
 
     Returns:
-        2D array: chord geometric matrix (Nlayer, Nlayer)
-    """
-    radius_roll = jnp.roll(radius, 1)
+        2D array: chord geometric matrix (Nlayer, Nlayer), lower triangle matrix
 
-    # elements at the top layer to be zero
-    radius_roll = radius_roll.at[0].set(radius[0])
-    height = height.at[0].set(jnp.inf)
-
-    fac_right = jnp.sqrt(radius[None, :]**2 - radius[:, None]**2)
-    fac_left = jnp.sqrt(radius_roll[None, :]**2 - radius[:, None]**2)
-    raw_matrix = 2.0*(fac_left - fac_right) / height
+    Notes:
+        Our definitions of the radius_lower and height (and radius_top, internally defined) are as follows:
+        n=0,1,...,N-1
+        radius_lower[N-1] = radius_btm (i.e. R0)    
+        radius_lower[n-1] = radius_lower[n] + height[n]
+        radius_top = radius_lower[0] + height[0]
+        
+    """
+    radius_top = radius_lower[0] + height[0]  #radius at TOA
+    radius_shifted = jnp.roll(radius_lower, 1)  # r_{k-1}
+    radius_shifted = radius_shifted.at[0].set(radius_top)
+    fac_right = jnp.sqrt(radius_lower[None, :]**2 - radius_lower[:, None]**2)
+    fac_left = jnp.sqrt(radius_shifted[None, :]**2 - radius_lower[:, None]**2)
+    raw_matrix = 2.0 * (fac_left - fac_right) / height
     return jnp.tril(raw_matrix)
 
 
-def tauchord(chord_geometric_matrix, xsmatrix):
-    """chord opacity vector from a chord geometric matrix and xsmatrix
+def chord_optical_depth(chord_geometric_matrix, dtau):
+    """chord optical depth vector from a chord geometric matrix and dtau
     
     Args:
         chord_geometric_matrix (jnp array): chord geometric matrix (Nlayer, Nlayer), lower triangle matrix 
-        xsmatrix (jnp array): cross section matrix (Nlayer, N_wavenumber)
+        dtau (jnp array): layer optical depth matrix, dtau (Nlayer, N_wavenumber)
 
-    Returns: tauchord matrix (Nlayer, N_wavenumber)
+    Returns: chord optical depth (tauchord) matrix (Nlayer, N_wavenumber)
 
     """
-    return jnp.dot(chord_geometric_matrix, xsmatrix)
+    return jnp.dot(chord_geometric_matrix, dtau)
```

## exojax/spec/set_ditgrid.py

```diff
@@ -44,15 +44,15 @@
 
     Returns:
         grid for DIT
     """
     if weight is None:
         weight = 1.0
 
-    assert np.min(weight * input_variable) > 0.0, "There exists negative or zero value. Consider to use np.abs."        
+    #assert np.min(weight * input_variable) > 0.0, "There exists negative or zero value. Consider to use np.abs."        
     wxmin = np.min(weight * input_variable)
     wxmax = np.max(weight * input_variable)
     wxmax = np.nextafter(wxmax, np.inf, dtype=wxmax.dtype)
     dwx = wxmax-wxmin
     Ng = int(dwx/dit_grid_resolution)+2
     if adopt == False:
         grid = np.linspace(wxmin, wxmin+(Ng-1)*dit_grid_resolution, Ng)
```

## exojax/spec/__pycache__/__init__.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 484 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 e401 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 e566 1664 e401 0000  U........f.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6700  .....@...s`...g.
 00000030: 5a00 6400 5a01 6401 5a02 6402 5a03 6403  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6401 5a05 6404 5a06 6405 6406 6c07  Z.d.Z.d.Z.d.d.l.
 00000050: 6d08 5a08 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6405 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 0100 6405  m.Z.m.Z.m.Z...d.
```

## exojax/spec/__pycache__/api.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 39886 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 ce9b 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 ce9b 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6403 6c05 6d03 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6403 6c07 5a07 6401 6403 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a08 6401 6403 6c09 5a09 6401 6404 6c0a  Z.d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0a 6d0c 5a0d  m.Z...d.d.l.m.Z.
```

## exojax/spec/__pycache__/atmrt.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 6910 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 fe1a 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 fe1a 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6402 6c0d 6d01 5a0e 0100 6401  ..d.d.l.m.Z...d.
```

## exojax/spec/__pycache__/dit.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 11359 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 5f2c 0000  U.......!..d_,..
+00000000: 550d 0d0a 0000 0000 e566 1664 5f2c 0000  U........f.d_,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 6d02 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6401 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

## exojax/spec/__pycache__/dtau_mmwl.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Mar 11 22:28:06 2023 UTC, .py size: 3560 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7600 0d64 e80d 0000  U.......v..d....
+00000000: 550d 0d0a 0000 0000 9c57 2d64 e80d 0000  U........W-d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6401 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6401 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0a 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

## exojax/spec/__pycache__/hitran.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 3546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 da0d 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 e566 1664 da0d 0000  U........f.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6400 6402 6c03 5a05 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c06 6d09 5a09 0100 6405 6406 8400  d.l.m.Z...d.d...
 00000070: 5a0a 6501 6407 6406 8400 8301 5a0a 6508  Z.e.d.d.....Z.e.
```

## exojax/spec/__pycache__/initspec.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 9355 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 8b24 0000  U.......!..d.$..
+00000000: 550d 0d0a 0000 0000 f75d 7864 8b24 0000  U........]xd.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6402 6c02 5a04 6401 6402 6c05 5a05 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c06 6d07 5a07 0100 6401 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

## exojax/spec/__pycache__/layeropacity.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Mar 11 22:55:38 2023 UTC, .py size: 3899 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,246 +1,259 @@
-00000000: 550d 0d0a 0000 0000 ea06 0d64 3b0f 0000  U..........d;...
+00000000: 550d 0d0a 0000 0000 9c57 2d64 7b10 0000  U........W-d{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6401 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
 00000080: 0100 6401 6408 6c0d 6d10 5a10 0100 6401  ..d.d.l.m.Z...d.
 00000090: 6409 6c11 6d12 5a12 0100 640a 640b 8400  d.l.m.Z...d.d...
 000000a0: 5a13 640c 640d 8400 5a14 640e 640f 8400  Z.d.d...Z.d.d...
 000000b0: 5a15 6410 6411 8400 5a16 6403 5300 2912  Z.d.d...Z.d.S.).
-000000c0: 7a32 636f 6d70 7574 6520 6f70 6163 6974  z2compute opacit
-000000d0: 7920 6469 6666 6572 656e 6365 2069 6e20  y difference in 
-000000e0: 6174 6d6f 7370 6865 7269 6320 6c61 7965  atmospheric laye
-000000f0: 7273 0a0a e900 0000 0029 02da 036a 6974  rs.......)...jit
-00000100: da04 766d 6170 4e29 01da 1569 6e74 6572  ..vmapN)...inter
-00000110: 705f 6c6f 6761 6369 615f 6d61 7472 6978  p_logacia_matrix
-00000120: 2901 da14 6c6f 675f 686d 696e 7573 5f63  )...log_hminus_c
-00000130: 6f6e 7469 6e75 756d 2901 da0e 6e75 6d62  ontinuum)...numb
-00000140: 6572 5f64 656e 7369 7479 2902 da05 6c6f  er_density)...lo
-00000150: 676b 42da 096c 6f67 6d5f 7563 6773 a901  gkB..logm_ucgs..
-00000160: da05 6f70 6661 6329 01da 0a64 7461 754d  ..opfac)...dtauM
-00000170: 5f6d 6d77 6c63 0500 0000 0000 0000 0000  _mmwlc..........
-00000180: 0000 0500 0000 0400 0000 4300 0000 7330  ..........C...s0
-00000190: 0000 0074 007c 0114 007c 0064 0164 0185  ...t.|...|.d.d..
-000001a0: 0264 0166 0219 0014 007c 0264 0164 0185  .d.f.....|.d.d..
-000001b0: 0264 0166 0219 0014 007c 037c 0414 001b  .d.f.....|.|....
-000001c0: 0053 0029 0261 0c02 0000 6474 6175 206f  .S.).a....dtau o
-000001d0: 6620 7468 6520 6d6f 6c65 6375 6c61 7220  f the molecular 
-000001e0: 6372 6f73 7320 7365 6374 696f 6e2e 0a0a  cross section...
-000001f0: 2020 2020 4e6f 7465 3a0a 2020 2020 2020      Note:.      
-00000200: 206f 7066 6163 3d62 6172 5f63 6773 2f28   opfac=bar_cgs/(
-00000210: 6d5f 7520 2867 2929 2e20 6d5f 753a 2061  m_u (g)). m_u: a
-00000220: 746f 6d69 6320 6d61 7373 2075 6e69 742e  tomic mass unit.
-00000230: 2049 7420 6361 6e20 6265 206f 6274 6169   It can be obtai
-00000240: 6e65 6420 6279 2066 6163 3d31 2e65 332f  ned by fac=1.e3/
-00000250: 6d5f 752c 2077 6865 7265 206d 5f75 203d  m_u, where m_u =
-00000260: 2073 6369 7079 2e63 6f6e 7374 616e 7473   scipy.constants
-00000270: 2e6d 5f75 2e0a 0a20 2020 2041 7267 733a  .m_u...    Args:
-00000280: 0a20 2020 2020 2020 6450 6172 723a 2064  .       dParr: d
-00000290: 656c 7461 2070 7265 7373 7572 6520 7072  elta pressure pr
-000002a0: 6f66 696c 6520 2862 6172 2920 5b4e 5f6c  ofile (bar) [N_l
-000002b0: 6179 6572 5d0a 2020 2020 2020 2078 736d  ayer].       xsm
-000002c0: 3a20 6372 6f73 7320 7365 6374 696f 6e20  : cross section 
-000002d0: 6d61 7472 6978 2028 636d 3229 205b 4e5f  matrix (cm2) [N_
-000002e0: 6c61 7965 722c 204e 5f6e 7573 5d0a 2020  layer, N_nus].  
-000002f0: 2020 2020 204d 523a 2076 6f6c 756d 6520       MR: volume 
-00000300: 6d69 7869 6e67 2072 6174 696f 2028 564d  mixing ratio (VM
-00000310: 5229 206f 7220 6d61 7373 206d 6978 696e  R) or mass mixin
-00000320: 6720 7261 7469 6f20 284d 4d52 2920 5b4e  g ratio (MMR) [N
-00000330: 5f6c 6179 6572 5d0a 2020 2020 2020 206d  _layer].       m
-00000340: 6173 733a 206d 6561 6e20 6d6f 6c65 6375  ass: mean molecu
-00000350: 6c61 7220 7765 6967 6874 2066 6f72 2056  lar weight for V
-00000360: 4d52 206f 7220 6d6f 6c65 6375 6c61 7220  MR or molecular 
-00000370: 6d61 7373 2066 6f72 204d 4d52 0a20 2020  mass for MMR.   
-00000380: 2020 2020 673a 2067 7261 7669 7479 2028      g: gravity (
-00000390: 636d 2f73 3229 0a0a 2020 2020 5265 7475  cm/s2)..    Retu
-000003a0: 726e 733a 0a20 2020 2020 2020 6f70 7469  rns:.       opti
-000003b0: 6361 6c20 6465 7074 6820 6d61 7472 6978  cal depth matrix
-000003c0: 205b 4e5f 6c61 7965 722c 204e 5f6e 7573   [N_layer, N_nus
-000003d0: 5d0a 2020 2020 4e72 0900 0000 2905 da05  ].    Nr....)...
-000003e0: 6450 6172 72da 0378 736d 5a02 4d52 5a04  dParr..xsmZ.MRZ.
-000003f0: 6d61 7373 da01 67a9 0072 0f00 0000 fa38  mass..g..r.....8
-00000400: 6275 696c 642f 6264 6973 742e 6c69 6e75  build/bdist.linu
-00000410: 782d 7838 365f 3634 2f65 6767 2f65 786f  x-x86_64/egg/exo
-00000420: 6a61 782f 7370 6563 2f6c 6179 6572 6f70  jax/spec/layerop
-00000430: 6163 6974 792e 7079 da13 6c61 7965 725f  acity.py..layer_
-00000440: 6f70 7469 6361 6c5f 6465 7074 680f 0000  optical_depth...
-00000450: 0073 0200 0000 0011 7211 0000 0063 0b00  .s......r....c..
-00000460: 0000 0000 0000 0000 0000 1100 0000 0700  ................
-00000470: 0000 4300 0000 73a0 0000 0074 007c 027c  ..C...s....t.|.|
-00000480: 0183 027d 0b74 01a0 027c 047c 0b14 00a1  ...}.t...|.|....
-00000490: 017d 0c74 01a0 027c 057c 0b14 00a1 017d  .}.t...|.|.....}
-000004a0: 0d74 01a0 027c 07a1 017d 0e7c 037c 021b  .t...|...}.|.|..
-000004b0: 007d 0f64 0174 037c 017c 007c 087c 097c  .}.d.t.|.|.|.|.|
-000004c0: 0a83 057c 0c64 0264 0285 0264 0266 0219  ...|.d.d...d.f..
-000004d0: 0017 007c 0d64 0264 0285 0264 0266 0219  ...|.d.d...d.f..
-000004e0: 0017 0074 0417 007c 0e18 0074 0518 0013  ...t...|...t....
-000004f0: 007c 0164 0264 0285 0264 0266 0219 0014  .|.d.d...d.f....
-00000500: 007c 061b 007c 0f64 0264 0285 0264 0266  .|...|.d.d...d.f
-00000510: 0219 0014 007d 107c 1053 0029 0361 5d02  .....}.|.S.).a].
-00000520: 0000 6474 6175 206f 6620 7468 6520 4349  ..dtau of the CI
-00000530: 4120 636f 6e74 696e 7575 6d2e 204e 6f74  A continuum. Not
-00000540: 2075 7365 6420 696e 2061 7274 2e0a 0a20   used in art... 
-00000550: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00000560: 6e75 733a 2077 6176 656e 756d 6265 7220  nus: wavenumber 
-00000570: 6d61 7472 6978 2028 636d 2d31 290a 2020  matrix (cm-1).  
-00000580: 2020 2020 2054 6172 723a 2074 656d 7065       Tarr: tempe
-00000590: 7261 7475 7265 2061 7272 6179 2028 4b29  rature array (K)
-000005a0: 0a20 2020 2020 2020 5061 7272 3a20 7465  .       Parr: te
-000005b0: 6d70 6572 6174 7572 6520 6172 7261 7920  mperature array 
-000005c0: 2862 6172 290a 2020 2020 2020 2064 5061  (bar).       dPa
-000005d0: 7272 3a20 6465 6c74 6120 7465 6d70 6572  rr: delta temper
-000005e0: 6174 7572 6520 6172 7261 7920 2862 6172  ature array (bar
-000005f0: 290a 2020 2020 2020 2076 6d72 313a 2076  ).       vmr1: v
-00000600: 6f6c 756d 6520 6d69 7869 6e67 2072 6174  olume mixing rat
-00000610: 696f 2028 564d 5229 2066 6f72 206d 6f6c  io (VMR) for mol
-00000620: 6563 756c 6573 2031 205b 4e5f 6c61 7965  ecules 1 [N_laye
-00000630: 725d 0a20 2020 2020 2020 766d 7232 3a20  r].       vmr2: 
-00000640: 766f 6c75 6d65 206d 6978 696e 6720 7261  volume mixing ra
-00000650: 7469 6f20 2856 4d52 2920 666f 7220 6d6f  tio (VMR) for mo
-00000660: 6c65 6375 6c65 7320 3220 5b4e 5f6c 6179  lecules 2 [N_lay
-00000670: 6572 5d0a 2020 2020 2020 206d 6d77 3a20  er].       mmw: 
-00000680: 6d65 616e 206d 6f6c 6563 756c 6172 2077  mean molecular w
-00000690: 6569 6768 7420 6f66 2061 746d 6f73 7068  eight of atmosph
-000006a0: 6572 650a 2020 2020 2020 2067 3a20 6772  ere.       g: gr
-000006b0: 6176 6974 7920 2863 6d32 2f73 290a 2020  avity (cm2/s).  
-000006c0: 2020 2020 206e 7563 6961 3a20 7761 7665       nucia: wave
-000006d0: 6e75 6d62 6572 2061 7272 6179 2066 6f72  number array for
-000006e0: 2043 4941 0a20 2020 2020 2020 7463 6961   CIA.       tcia
-000006f0: 3a20 7465 6d70 6572 6174 7572 6520 6172  : temperature ar
-00000700: 7261 7920 666f 7220 4349 410a 2020 2020  ray for CIA.    
-00000710: 2020 206c 6f67 6163 3a20 6c6f 6731 3028     logac: log10(
-00000720: 6162 736f 7270 7469 6f6e 2063 6f65 6666  absorption coeff
-00000730: 6963 6965 6e74 206f 6620 4349 4129 0a0a  icient of CIA)..
-00000740: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00000750: 2020 2020 6f70 7469 6361 6c20 6465 7074      optical dept
-00000760: 6820 6d61 7472 6978 2020 5b4e 5f6c 6179  h matrix  [N_lay
-00000770: 6572 2c20 4e5f 6e75 735d 0a20 2020 20e9  er, N_nus].    .
-00000780: 0a00 0000 4e29 0672 0600 0000 da03 6a6e  ....N).r......jn
-00000790: 70da 056c 6f67 3130 7204 0000 0072 0700  p..log10r....r..
-000007a0: 0000 7208 0000 0029 11da 036e 7573 da04  ..r....)...nus..
-000007b0: 5461 7272 da04 5061 7272 720c 0000 005a  Tarr..Parrr....Z
-000007c0: 0476 6d72 315a 0476 6d72 32da 036d 6d77  .vmr1Z.vmr2..mmw
-000007d0: 720e 0000 005a 056e 7563 6961 5a04 7463  r....Z.nuciaZ.tc
-000007e0: 6961 5a05 6c6f 6761 63da 046e 6172 725a  iaZ.logac..narrZ
-000007f0: 086c 6f67 6e61 7272 315a 086c 6f67 6e61  .lognarr1Z.logna
-00000800: 7272 32da 046c 6f67 67da 0664 6450 6172  rr2..logg..ddPar
-00000810: 725a 0564 7461 7563 720f 0000 0072 0f00  rZ.dtaucr....r..
-00000820: 0000 7210 0000 00da 176c 6179 6572 5f6f  ..r......layer_o
-00000830: 7074 6963 616c 5f64 6570 7468 5f43 4941  ptical_depth_CIA
-00000840: 2300 0000 732e 0000 0000 130a 010e 010e  #...s...........
-00000850: 010a 0108 0110 010e ff02 010e ff02 0102  ................
-00000860: ff02 0102 ff02 0202 fe04 020e fe02 0202  ................
-00000870: fe02 020e fe04 0472 1c00 0000 6305 0000  .......r....c...
-00000880: 0000 0000 0000 0000 0007 0000 0006 0000  ................
-00000890: 0043 0000 0073 3200 0000 7400 7401 7402  .C...s2...t.t.t.
-000008a0: 6401 8302 8301 7c00 7c01 7c02 7c03 7c04  d.....|.|.|.|.|.
-000008b0: 8305 7d05 7403 a004 7403 6a05 7c05 6402  ..}.t...t.j.|.d.
-000008c0: 6403 8d02 a101 7d06 7c06 5300 2904 617d  d.....}.|.S.).a}
-000008d0: 0100 0064 7461 7520 6f66 2074 6865 2061  ...dtau of the a
-000008e0: 746f 6d69 6320 282b 696f 6e69 6329 2063  tomic (+ionic) c
-000008f0: 726f 7373 2073 6563 7469 6f6e 2066 726f  ross section fro
-00000900: 6d20 5641 4c44 2e0a 0a20 2020 2041 7267  m VALD...    Arg
-00000910: 733a 0a20 2020 2020 2020 6450 6172 723a  s:.       dParr:
-00000920: 2064 656c 7461 2070 7265 7373 7572 6520   delta pressure 
-00000930: 7072 6f66 696c 6520 2862 6172 2920 5b4e  profile (bar) [N
-00000940: 5f6c 6179 6572 5d0a 2020 2020 2020 2078  _layer].       x
-00000950: 736d 3a20 6372 6f73 7320 7365 6374 696f  sm: cross sectio
-00000960: 6e20 6d61 7472 6978 2028 636d 3229 205b  n matrix (cm2) [
-00000970: 4e5f 7370 6563 6965 7320 7820 4e5f 6c61  N_species x N_la
-00000980: 7965 7220 7820 4e5f 7761 765d 0a20 2020  yer x N_wav].   
-00000990: 2020 2020 564d 523a 2076 6f6c 756d 6520      VMR: volume 
-000009a0: 6d69 7869 6e67 2072 6174 696f 205b 4e5f  mixing ratio [N_
-000009b0: 7370 6563 6965 7320 7820 4e5f 6c61 7965  species x N_laye
-000009c0: 725d 0a20 2020 2020 2020 6d6d 773a 206d  r].       mmw: m
-000009d0: 6561 6e20 6d6f 6c65 6375 6c61 7220 7765  ean molecular we
-000009e0: 6967 6874 205b 4e5f 6c61 7965 725d 0a20  ight [N_layer]. 
-000009f0: 2020 2020 2020 673a 2067 7261 7669 7479        g: gravity
-00000a00: 2028 636d 2f73 3229 0a0a 2020 2020 5265   (cm/s2)..    Re
-00000a10: 7475 726e 733a 0a20 2020 2020 2020 2064  turns:.        d
-00000a20: 7461 753a 206f 7074 6963 616c 2064 6570  tau: optical dep
-00000a30: 7468 206d 6174 7269 7820 5b4e 5f6c 6179  th matrix [N_lay
-00000a40: 6572 2078 204e 5f6e 7573 5d0a 2020 2020  er x N_nus].    
-00000a50: 2905 4e72 0100 0000 7201 0000 004e 4e72  ).Nr....r....NNr
-00000a60: 0100 0000 2901 5a04 6178 6973 2906 7202  ....).Z.axis).r.
-00000a70: 0000 0072 0300 0000 720b 0000 0072 1300  ...r....r....r..
-00000a80: 0000 da03 6162 73da 0373 756d 2907 720c  ....abs..sum).r.
-00000a90: 0000 0072 0d00 0000 5a03 564d 5272 1800  ...r....Z.VMRr..
-00000aa0: 0000 720e 0000 005a 0564 7461 7553 5a04  ..r....Z.dtauSZ.
-00000ab0: 6474 6175 720f 0000 0072 0f00 0000 7210  dtaur....r....r.
-00000ac0: 0000 00da 186c 6179 6572 5f6f 7074 6963  .....layer_optic
-00000ad0: 616c 5f64 6570 7468 5f56 414c 4442 0000  al_depth_VALDB..
-00000ae0: 0073 1200 0000 000d 0c01 0200 0200 0200  .s..............
-00000af0: 0200 02ff 0402 1401 721f 0000 0063 0800  ........r....c..
-00000b00: 0000 0000 0000 0000 0000 0f00 0000 0500  ................
-00000b10: 0000 4300 0000 7376 0000 0074 007c 027c  ..C...sv...t.|.|
-00000b20: 0183 027d 087c 047c 0814 007d 097c 057c  ...}.|.|...}.|.|
-00000b30: 0814 007d 0a74 01a0 027c 07a1 017d 0b7c  ...}.t...|...}.|
-00000b40: 037c 021b 007d 0c74 037c 007c 017c 097c  .|...}.t.|.|.|.|
-00000b50: 0a83 047d 0d64 017c 0d74 0417 007c 0b18  ...}.d.|.t...|..
-00000b60: 0074 0518 0013 007c 0164 0264 0285 0264  .t.....|.d.d...d
-00000b70: 0266 0219 0014 007c 061b 007c 0c64 0264  .f.....|...|.d.d
-00000b80: 0285 0264 0266 0219 0014 007d 0e7c 0e53  ...d.f.....}.|.S
-00000b90: 0029 0361 bd01 0000 6474 6175 206f 6620  .).a....dtau of 
-00000ba0: 7468 6520 482d 2063 6f6e 7469 6e75 756d  the H- continuum
-00000bb0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00000bc0: 2020 2020 6e75 733a 2077 6176 656e 756d      nus: wavenum
-00000bd0: 6265 7220 6d61 7472 6978 2028 636d 2d31  ber matrix (cm-1
-00000be0: 290a 2020 2020 2020 2054 6172 723a 2074  ).       Tarr: t
-00000bf0: 656d 7065 7261 7475 7265 2061 7272 6179  emperature array
-00000c00: 2028 4b29 0a20 2020 2020 2020 5061 7272   (K).       Parr
-00000c10: 3a20 7465 6d70 6572 6174 7572 6520 6172  : temperature ar
-00000c20: 7261 7920 2862 6172 290a 2020 2020 2020  ray (bar).      
-00000c30: 2064 5061 7272 3a20 6465 6c74 6120 7465   dParr: delta te
-00000c40: 6d70 6572 6174 7572 6520 6172 7261 7920  mperature array 
-00000c50: 2862 6172 290a 2020 2020 2020 2076 6d72  (bar).       vmr
-00000c60: 653a 2076 6f6c 756d 6520 6d69 7869 6e67  e: volume mixing
-00000c70: 2072 6174 696f 2028 564d 5229 2066 6f72   ratio (VMR) for
-00000c80: 2065 2d20 5b4e 5f6c 6179 6572 5d0a 2020   e- [N_layer].  
-00000c90: 2020 2020 2076 6d72 483a 2076 6f6c 756d       vmrH: volum
-00000ca0: 6520 6d69 7869 6e67 2072 6174 696f 2028  e mixing ratio (
-00000cb0: 564d 5229 2066 6f72 2048 2061 746f 6d73  VMR) for H atoms
-00000cc0: 205b 4e5f 6c61 7965 725d 0a20 2020 2020   [N_layer].     
-00000cd0: 2020 6d6d 773a 206d 6561 6e20 6d6f 6c65    mmw: mean mole
-00000ce0: 6375 6c61 7220 7765 6967 6874 206f 6620  cular weight of 
-00000cf0: 6174 6d6f 7370 6865 7265 0a20 2020 2020  atmosphere.     
-00000d00: 2020 673a 2067 7261 7669 7479 2028 636d    g: gravity (cm
-00000d10: 322f 7329 0a0a 2020 2020 5265 7475 726e  2/s)..    Return
-00000d20: 733a 0a20 2020 2020 2020 6f70 7469 6361  s:.       optica
-00000d30: 6c20 6465 7074 6820 6d61 7472 6978 2020  l depth matrix  
-00000d40: 5b4e 5f6c 6179 6572 2c20 4e5f 6e75 735d  [N_layer, N_nus]
-00000d50: 0a20 2020 2072 1200 0000 4e29 0672 0600  .    r....N).r..
-00000d60: 0000 7213 0000 0072 1400 0000 7205 0000  ..r....r....r...
-00000d70: 0072 0700 0000 7208 0000 0029 0f72 1500  .r....r....).r..
-00000d80: 0000 7216 0000 0072 1700 0000 720c 0000  ..r....r....r...
-00000d90: 005a 0476 6d72 655a 0476 6d72 6872 1800  .Z.vmreZ.vmrhr..
-00000da0: 0000 720e 0000 0072 1900 0000 5a10 6e75  ..r....r....Z.nu
-00000db0: 6d62 6572 5f64 656e 7369 7479 5f65 5a10  mber_density_eZ.
-00000dc0: 6e75 6d62 6572 5f64 656e 7369 7479 5f68  number_density_h
-00000dd0: 721a 0000 0072 1b00 0000 5a06 6c6f 6761  r....r....Z.loga
-00000de0: 6263 5a05 6474 6175 6872 0f00 0000 720f  bcZ.dtauhr....r.
-00000df0: 0000 0072 1000 0000 da1a 6c61 7965 725f  ...r......layer_
-00000e00: 6f70 7469 6361 6c5f 6465 7074 685f 486d  optical_depth_Hm
-00000e10: 696e 7573 5500 0000 7324 0000 0000 100a  inusU...s$......
-00000e20: 0308 0108 010a 0108 0108 0102 ff04 020c  ................
-00000e30: 0102 ff04 010e ff02 0102 ff02 010e ff04  ................
-00000e40: 0372 2000 0000 2917 da07 5f5f 646f 635f  .r ...)...__doc_
-00000e50: 5f5a 036a 6178 7202 0000 0072 0300 0000  _Z.jaxr....r....
-00000e60: 5a09 6a61 782e 6e75 6d70 79da 056e 756d  Z.jax.numpy..num
-00000e70: 7079 7213 0000 005a 1565 786f 6a61 782e  pyr....Z.exojax.
-00000e80: 7370 6563 2e68 6974 7261 6e63 6961 7204  spec.hitranciar.
-00000e90: 0000 005a 1265 786f 6a61 782e 7370 6563  ...Z.exojax.spec
-00000ea0: 2e68 6d69 6e75 7372 0500 0000 5a13 6578  .hminusr....Z.ex
-00000eb0: 6f6a 6178 2e61 746d 2e69 6465 616c 6761  ojax.atm.idealga
-00000ec0: 7372 0600 0000 5a16 6578 6f6a 6178 2e75  sr....Z.exojax.u
-00000ed0: 7469 6c73 2e63 6f6e 7374 616e 7473 7207  tils.constantsr.
-00000ee0: 0000 0072 0800 0000 720a 0000 005a 1565  ...r....r....Z.e
-00000ef0: 786f 6a61 782e 7370 6563 2e64 7461 755f  xojax.spec.dtau_
-00000f00: 6d6d 776c 720b 0000 0072 1100 0000 721c  mmwlr....r....r.
-00000f10: 0000 0072 1f00 0000 7220 0000 0072 0f00  ...r....r ...r..
-00000f20: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000f30: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000f40: 1800 0000 0404 1001 0c01 0c01 0c01 0c01  ................
-00000f50: 1001 0c01 0c03 0814 081f 0813            ............
+000000c0: 7a33 2063 6f6d 7075 7465 206f 7061 6369  z3 compute opaci
+000000d0: 7479 2064 6966 6665 7265 6e63 6520 696e  ty difference in
+000000e0: 2061 746d 6f73 7068 6572 6963 206c 6179   atmospheric lay
+000000f0: 6572 730a 0ae9 0000 0000 2902 da03 6a69  ers.......)...ji
+00000100: 74da 0476 6d61 704e 2901 da15 696e 7465  t..vmapN)...inte
+00000110: 7270 5f6c 6f67 6163 6961 5f6d 6174 7269  rp_logacia_matri
+00000120: 7829 01da 146c 6f67 5f68 6d69 6e75 735f  x)...log_hminus_
+00000130: 636f 6e74 696e 7575 6d29 01da 0e6e 756d  continuum)...num
+00000140: 6265 725f 6465 6e73 6974 7929 02da 056c  ber_density)...l
+00000150: 6f67 6b42 da09 6c6f 676d 5f75 6367 73a9  ogkB..logm_ucgs.
+00000160: 01da 056f 7066 6163 2901 da0a 6474 6175  ...opfac)...dtau
+00000170: 4d5f 6d6d 776c 6305 0000 0000 0000 0000  M_mmwlc.........
+00000180: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
+00000190: 3000 0000 7400 7c01 1400 7c00 6401 6401  0...t.|...|.d.d.
+000001a0: 8502 6401 6602 1900 1400 7c02 6401 6401  ..d.f.....|.d.d.
+000001b0: 8502 6401 6602 1900 1400 7c03 7c04 1400  ..d.f.....|.|...
+000001c0: 1b00 5300 2902 6139 0200 0064 7461 7520  ..S.).a9...dtau 
+000001d0: 6f66 2074 6865 206d 6f6c 6563 756c 6172  of the molecular
+000001e0: 2063 726f 7373 2073 6563 7469 6f6e 2e0a   cross section..
+000001f0: 0a20 2020 204e 6f74 653a 0a20 2020 2020  .    Note:.     
+00000200: 2020 206f 7066 6163 3d62 6172 5f63 6773     opfac=bar_cgs
+00000210: 2f28 6d5f 7520 2867 2929 2e20 6d5f 753a  /(m_u (g)). m_u:
+00000220: 2061 746f 6d69 6320 6d61 7373 2075 6e69   atomic mass uni
+00000230: 742e 2049 7420 6361 6e20 6265 206f 6274  t. It can be obt
+00000240: 6169 6e65 6420 6279 2066 6163 3d31 2e65  ained by fac=1.e
+00000250: 332f 6d5f 752c 2077 6865 7265 206d 5f75  3/m_u, where m_u
+00000260: 203d 2073 6369 7079 2e63 6f6e 7374 616e   = scipy.constan
+00000270: 7473 2e6d 5f75 2e0a 0a20 2020 2041 7267  ts.m_u...    Arg
+00000280: 733a 0a20 2020 2020 2020 2064 5061 7272  s:.        dParr
+00000290: 3a20 6465 6c74 6120 7072 6573 7375 7265  : delta pressure
+000002a0: 2070 726f 6669 6c65 2028 6261 7229 205b   profile (bar) [
+000002b0: 4e5f 6c61 7965 725d 0a20 2020 2020 2020  N_layer].       
+000002c0: 2078 736d 6174 7269 783a 2063 726f 7373   xsmatrix: cross
+000002d0: 2073 6563 7469 6f6e 206d 6174 7269 7820   section matrix 
+000002e0: 2863 6d32 2920 5b4e 5f6c 6179 6572 2c20  (cm2) [N_layer, 
+000002f0: 4e5f 6e75 735d 0a20 2020 2020 2020 206d  N_nus].        m
+00000300: 6978 696e 675f 7261 7469 6f3a 2076 6f6c  ixing_ratio: vol
+00000310: 756d 6520 6d69 7869 6e67 2072 6174 696f  ume mixing ratio
+00000320: 2028 564d 5229 206f 7220 6d61 7373 206d   (VMR) or mass m
+00000330: 6978 696e 6720 7261 7469 6f20 284d 4d52  ixing ratio (MMR
+00000340: 2920 5b4e 5f6c 6179 6572 5d0a 2020 2020  ) [N_layer].    
+00000350: 2020 2020 6d61 7373 3a20 6d65 616e 206d      mass: mean m
+00000360: 6f6c 6563 756c 6172 2077 6569 6768 7420  olecular weight 
+00000370: 666f 7220 564d 5220 6f72 206d 6f6c 6563  for VMR or molec
+00000380: 756c 6172 206d 6173 7320 666f 7220 4d4d  ular mass for MM
+00000390: 520a 2020 2020 2020 2020 6772 6176 6974  R.        gravit
+000003a0: 793a 2067 7261 7669 7479 2028 636d 2f73  y: gravity (cm/s
+000003b0: 3229 0a0a 2020 2020 5265 7475 726e 733a  2)..    Returns:
+000003c0: 0a20 2020 2020 2020 2032 4420 6172 7261  .        2D arra
+000003d0: 793a 206f 7074 6963 616c 2064 6570 7468  y: optical depth
+000003e0: 206d 6174 7269 782c 2064 7461 7520 205b   matrix, dtau  [
+000003f0: 4e5f 6c61 7965 722c 204e 5f6e 7573 5d0a  N_layer, N_nus].
+00000400: 2020 2020 4e72 0900 0000 2905 da05 6450      Nr....)...dP
+00000410: 6172 725a 0878 736d 6174 7269 785a 0c6d  arrZ.xsmatrixZ.m
+00000420: 6978 696e 675f 7261 7469 6f5a 046d 6173  ixing_ratioZ.mas
+00000430: 73da 0767 7261 7669 7479 a900 720e 0000  s..gravity..r...
+00000440: 00fa 3862 7569 6c64 2f62 6469 7374 2e6c  ..8build/bdist.l
+00000450: 696e 7578 2d78 3836 5f36 342f 6567 672f  inux-x86_64/egg/
+00000460: 6578 6f6a 6178 2f73 7065 632f 6c61 7965  exojax/spec/laye
+00000470: 726f 7061 6369 7479 2e70 79da 136c 6179  ropacity.py..lay
+00000480: 6572 5f6f 7074 6963 616c 5f64 6570 7468  er_optical_depth
+00000490: 0f00 0000 7306 0000 0000 1126 0106 ff72  ....s......&...r
+000004a0: 1000 0000 630b 0000 0000 0000 0000 0000  ....c...........
+000004b0: 0011 0000 0007 0000 0043 0000 0073 a000  .........C...s..
+000004c0: 0000 7400 7c02 7c01 8302 7d0b 7401 a002  ..t.|.|...}.t...
+000004d0: 7c04 7c0b 1400 a101 7d0c 7401 a002 7c05  |.|.....}.t...|.
+000004e0: 7c0b 1400 a101 7d0d 7401 a002 7c07 a101  |.....}.t...|...
+000004f0: 7d0e 7c03 7c02 1b00 7d0f 6401 7403 7c01  }.|.|...}.d.t.|.
+00000500: 7c00 7c08 7c09 7c0a 8305 7c0c 6402 6402  |.|.|.|...|.d.d.
+00000510: 8502 6402 6602 1900 1700 7c0d 6402 6402  ..d.f.....|.d.d.
+00000520: 8502 6402 6602 1900 1700 7404 1700 7c0e  ..d.f.....t...|.
+00000530: 1800 7405 1800 1300 7c01 6402 6402 8502  ..t.....|.d.d...
+00000540: 6402 6602 1900 1400 7c06 1b00 7c0f 6402  d.f.....|...|.d.
+00000550: 6402 8502 6402 6602 1900 1400 7d10 7c10  d...d.f.....}.|.
+00000560: 5300 2903 6185 0200 0064 7461 7520 6f66  S.).a....dtau of
+00000570: 2074 6865 2043 4941 2063 6f6e 7469 6e75   the CIA continu
+00000580: 756d 2e20 4e6f 7420 7573 6564 2069 6e20  um. Not used in 
+00000590: 6172 742e 0a0a 2020 2020 4172 6773 3a0a  art...    Args:.
+000005a0: 2020 2020 2020 2020 6e75 5f67 7269 643a          nu_grid:
+000005b0: 2077 6176 656e 756d 6265 7220 6d61 7472   wavenumber matr
+000005c0: 6978 2028 636d 2d31 290a 2020 2020 2020  ix (cm-1).      
+000005d0: 2020 7465 6d70 6572 6174 7572 653a 2074    temperature: t
+000005e0: 656d 7065 7261 7475 7265 2061 7272 6179  emperature array
+000005f0: 2028 4b29 0a20 2020 2020 2020 2070 7265   (K).        pre
+00000600: 7373 7572 653a 2070 7265 7373 7572 6520  ssure: pressure 
+00000610: 6172 7261 7920 2862 6172 290a 2020 2020  array (bar).    
+00000620: 2020 2020 6450 6172 723a 2064 656c 7461      dParr: delta
+00000630: 2074 656d 7065 7261 7475 7265 2061 7272   temperature arr
+00000640: 6179 2028 6261 7229 0a20 2020 2020 2020  ay (bar).       
+00000650: 2076 6d72 313a 2076 6f6c 756d 6520 6d69   vmr1: volume mi
+00000660: 7869 6e67 2072 6174 696f 2028 564d 5229  xing ratio (VMR)
+00000670: 2066 6f72 206d 6f6c 6563 756c 6573 2031   for molecules 1
+00000680: 205b 4e5f 6c61 7965 725d 0a20 2020 2020   [N_layer].     
+00000690: 2020 2076 6d72 323a 2076 6f6c 756d 6520     vmr2: volume 
+000006a0: 6d69 7869 6e67 2072 6174 696f 2028 564d  mixing ratio (VM
+000006b0: 5229 2066 6f72 206d 6f6c 6563 756c 6573  R) for molecules
+000006c0: 2032 205b 4e5f 6c61 7965 725d 0a20 2020   2 [N_layer].   
+000006d0: 2020 2020 206d 6d77 3a20 6d65 616e 206d       mmw: mean m
+000006e0: 6f6c 6563 756c 6172 2077 6569 6768 7420  olecular weight 
+000006f0: 6f66 2061 746d 6f73 7068 6572 650a 2020  of atmosphere.  
+00000700: 2020 2020 2020 673a 2067 7261 7669 7479        g: gravity
+00000710: 2028 636d 322f 7329 0a20 2020 2020 2020   (cm2/s).       
+00000720: 206e 7563 6961 3a20 7761 7665 6e75 6d62   nucia: wavenumb
+00000730: 6572 2061 7272 6179 2066 6f72 2043 4941  er array for CIA
+00000740: 0a20 2020 2020 2020 2074 6369 613a 2074  .        tcia: t
+00000750: 656d 7065 7261 7475 7265 2061 7272 6179  emperature array
+00000760: 2066 6f72 2043 4941 0a20 2020 2020 2020   for CIA.       
+00000770: 206c 6f67 6163 3a20 6c6f 6731 3028 6162   logac: log10(ab
+00000780: 736f 7270 7469 6f6e 2063 6f65 6666 6963  sorption coeffic
+00000790: 6965 6e74 206f 6620 4349 4129 0a0a 2020  ient of CIA)..  
+000007a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000007b0: 2020 2032 4420 6172 7261 793a 206f 7074     2D array: opt
+000007c0: 6963 616c 2064 6570 7468 206d 6174 7269  ical depth matri
+000007d0: 782c 2064 7461 7520 205b 4e5f 6c61 7965  x, dtau  [N_laye
+000007e0: 722c 204e 5f6e 7573 5d0a 2020 2020 e90a  r, N_nus].    ..
+000007f0: 0000 004e 2906 7206 0000 00da 036a 6e70  ...N).r......jnp
+00000800: da05 6c6f 6731 3072 0400 0000 7207 0000  ..log10r....r...
+00000810: 0072 0800 0000 2911 da07 6e75 5f67 7269  .r....)...nu_gri
+00000820: 64da 0b74 656d 7065 7261 7475 7265 5a08  d..temperatureZ.
+00000830: 7072 6573 7375 7265 720c 0000 005a 0476  pressurer....Z.v
+00000840: 6d72 315a 0476 6d72 32da 036d 6d77 da01  mr1Z.vmr2..mmw..
+00000850: 675a 056e 7563 6961 5a04 7463 6961 5a05  gZ.nuciaZ.tciaZ.
+00000860: 6c6f 6761 63da 046e 6172 725a 086c 6f67  logac..narrZ.log
+00000870: 6e61 7272 315a 086c 6f67 6e61 7272 32da  narr1Z.lognarr2.
+00000880: 046c 6f67 67da 0664 6450 6172 725a 0564  .logg..ddParrZ.d
+00000890: 7461 7563 720e 0000 0072 0e00 0000 720f  taucr....r....r.
+000008a0: 0000 00da 176c 6179 6572 5f6f 7074 6963  .....layer_optic
+000008b0: 616c 5f64 6570 7468 5f43 4941 2400 0000  al_depth_CIA$...
+000008c0: 7330 0000 0000 140a 010e 010e 010a 0108  s0..............
+000008d0: 0210 010e ff02 010e ff02 0102 ff02 0102  ................
+000008e0: ff02 0102 ff04 020e fe02 0202 fe02 020e  ................
+000008f0: fe02 ff02 0572 1b00 0000 6305 0000 0000  .....r....c.....
+00000900: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
+00000910: 0000 0073 3200 0000 7400 7401 7402 6401  ...s2...t.t.t.d.
+00000920: 8302 8301 7c00 7c01 7c02 7c03 7c04 8305  ....|.|.|.|.|...
+00000930: 7d05 7403 a004 7403 6a05 7c05 6402 6403  }.t...t.j.|.d.d.
+00000940: 8d02 a101 7d06 7c06 5300 2904 61a4 0100  ....}.|.S.).a...
+00000950: 0064 7461 7520 6f66 2074 6865 2061 746f  .dtau of the ato
+00000960: 6d69 6320 282b 696f 6e69 6329 2063 726f  mic (+ionic) cro
+00000970: 7373 2073 6563 7469 6f6e 2066 726f 6d20  ss section from 
+00000980: 5641 4c44 2e0a 0a20 2020 2041 7267 733a  VALD...    Args:
+00000990: 0a20 2020 2020 2020 2064 5061 7272 3a20  .        dParr: 
+000009a0: 6465 6c74 6120 7072 6573 7375 7265 2070  delta pressure p
+000009b0: 726f 6669 6c65 2028 6261 7229 205b 4e5f  rofile (bar) [N_
+000009c0: 6c61 7965 725d 0a20 2020 2020 2020 2078  layer].        x
+000009d0: 736d 3a20 6372 6f73 7320 7365 6374 696f  sm: cross sectio
+000009e0: 6e20 6d61 7472 6978 2028 636d 3229 205b  n matrix (cm2) [
+000009f0: 4e5f 7370 6563 6965 7320 7820 4e5f 6c61  N_species x N_la
+00000a00: 7965 7220 7820 4e5f 7761 765d 0a20 2020  yer x N_wav].   
+00000a10: 2020 2020 2056 4d52 3a20 766f 6c75 6d65       VMR: volume
+00000a20: 206d 6978 696e 6720 7261 7469 6f20 5b4e   mixing ratio [N
+00000a30: 5f73 7065 6369 6573 2078 204e 5f6c 6179  _species x N_lay
+00000a40: 6572 5d0a 2020 2020 2020 2020 6d65 616e  er].        mean
+00000a50: 5f6d 6f6c 6563 756c 6172 5f77 6569 6768  _molecular_weigh
+00000a60: 743a 206d 6561 6e20 6d6f 6c65 6375 6c61  t: mean molecula
+00000a70: 7220 7765 6967 6874 205b 4e5f 6c61 7965  r weight [N_laye
+00000a80: 725d 0a20 2020 2020 2020 2067 7261 7669  r].        gravi
+00000a90: 7479 3a20 6772 6176 6974 7920 2863 6d2f  ty: gravity (cm/
+00000aa0: 7332 290a 0a20 2020 2052 6574 7572 6e73  s2)..    Returns
+00000ab0: 3a0a 2020 2020 2020 2020 3244 2061 7272  :.        2D arr
+00000ac0: 6179 3a20 6f70 7469 6361 6c20 6465 7074  ay: optical dept
+00000ad0: 6820 6d61 7472 6978 2c20 6474 6175 2020  h matrix, dtau  
+00000ae0: 5b4e 5f6c 6179 6572 2c20 4e5f 6e75 735d  [N_layer, N_nus]
+00000af0: 0a20 2020 2029 054e 7201 0000 0072 0100  .    ).Nr....r..
+00000b00: 0000 4e4e 7201 0000 0029 015a 0461 7869  ..NNr....).Z.axi
+00000b10: 7329 0672 0200 0000 7203 0000 0072 0b00  s).r....r....r..
+00000b20: 0000 7212 0000 00da 0361 6273 da03 7375  ..r......abs..su
+00000b30: 6d29 0772 0c00 0000 5a03 7873 6d5a 0356  m).r....Z.xsmZ.V
+00000b40: 4d52 5a15 6d65 616e 5f6d 6f6c 6563 756c  MRZ.mean_molecul
+00000b50: 6172 5f77 6569 6768 7472 0d00 0000 5a05  ar_weightr....Z.
+00000b60: 6474 6175 535a 0464 7461 7572 0e00 0000  dtauSZ.dtaur....
+00000b70: 720e 0000 0072 0f00 0000 da18 6c61 7965  r....r......laye
+00000b80: 725f 6f70 7469 6361 6c5f 6465 7074 685f  r_optical_depth_
+00000b90: 5641 4c44 4500 0000 7312 0000 0000 0d0c  VALDE...s.......
+00000ba0: 0102 0002 0002 0002 0002 ff04 0214 0172  ...............r
+00000bb0: 1e00 0000 6308 0000 0000 0000 0000 0000  ....c...........
+00000bc0: 000f 0000 0005 0000 0043 0000 0073 7600  .........C...sv.
+00000bd0: 0000 7400 7c02 7c01 8302 7d08 7c04 7c08  ..t.|.|...}.|.|.
+00000be0: 1400 7d09 7c05 7c08 1400 7d0a 7401 a002  ..}.|.|...}.t...
+00000bf0: 7c07 a101 7d0b 7c03 7c02 1b00 7d0c 7403  |...}.|.|...}.t.
+00000c00: 7c00 7c01 7c09 7c0a 8304 7d0d 6401 7c0d  |.|.|.|...}.d.|.
+00000c10: 7404 1700 7c0b 1800 7405 1800 1300 7c01  t...|...t.....|.
+00000c20: 6402 6402 8502 6402 6602 1900 1400 7c06  d.d...d.f.....|.
+00000c30: 1b00 7c0c 6402 6402 8502 6402 6602 1900  ..|.d.d...d.f...
+00000c40: 1400 7d0e 7c0e 5300 2903 61ca 0100 0064  ..}.|.S.).a....d
+00000c50: 7461 7520 6f66 2074 6865 2048 2d20 636f  tau of the H- co
+00000c60: 6e74 696e 7575 6d2e 0a0a 2020 2020 4172  ntinuum...    Ar
+00000c70: 6773 3a0a 2020 2020 2020 2020 6e75 5f67  gs:.        nu_g
+00000c80: 7269 643a 2077 6176 656e 756d 6265 7220  rid: wavenumber 
+00000c90: 6d61 7472 6978 2028 636d 2d31 290a 2020  matrix (cm-1).  
+00000ca0: 2020 2020 2020 5461 7272 3a20 7465 6d70        Tarr: temp
+00000cb0: 6572 6174 7572 6520 6172 7261 7920 284b  erature array (K
+00000cc0: 290a 2020 2020 2020 2020 5061 7272 3a20  ).        Parr: 
+00000cd0: 7465 6d70 6572 6174 7572 6520 6172 7261  temperature arra
+00000ce0: 7920 2862 6172 290a 2020 2020 2020 2020  y (bar).        
+00000cf0: 6450 6172 723a 2064 656c 7461 2074 656d  dParr: delta tem
+00000d00: 7065 7261 7475 7265 2061 7272 6179 2028  perature array (
+00000d10: 6261 7229 0a20 2020 2020 2020 2076 6d72  bar).        vmr
+00000d20: 653a 2076 6f6c 756d 6520 6d69 7869 6e67  e: volume mixing
+00000d30: 2072 6174 696f 2028 564d 5229 2066 6f72   ratio (VMR) for
+00000d40: 2065 2d20 5b4e 5f6c 6179 6572 5d0a 2020   e- [N_layer].  
+00000d50: 2020 2020 2020 766d 7248 3a20 766f 6c75        vmrH: volu
+00000d60: 6d65 206d 6978 696e 6720 7261 7469 6f20  me mixing ratio 
+00000d70: 2856 4d52 2920 666f 7220 4820 6174 6f6d  (VMR) for H atom
+00000d80: 7320 5b4e 5f6c 6179 6572 5d0a 2020 2020  s [N_layer].    
+00000d90: 2020 2020 6d6d 773a 206d 6561 6e20 6d6f      mmw: mean mo
+00000da0: 6c65 6375 6c61 7220 7765 6967 6874 206f  lecular weight o
+00000db0: 6620 6174 6d6f 7370 6865 7265 0a20 2020  f atmosphere.   
+00000dc0: 2020 2020 2067 3a20 6772 6176 6974 7920       g: gravity 
+00000dd0: 2863 6d32 2f73 290a 0a20 2020 2052 6574  (cm2/s)..    Ret
+00000de0: 7572 6e73 3a0a 2020 2020 2020 2020 6f70  urns:.        op
+00000df0: 7469 6361 6c20 6465 7074 6820 6d61 7472  tical depth matr
+00000e00: 6978 2020 5b4e 5f6c 6179 6572 2c20 4e5f  ix  [N_layer, N_
+00000e10: 6e75 735d 0a20 2020 2072 1100 0000 4e29  nus].    r....N)
+00000e20: 0672 0600 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000e30: 7205 0000 0072 0700 0000 7208 0000 0029  r....r....r....)
+00000e40: 0f72 1400 0000 7215 0000 005a 0450 6172  .r....r....Z.Par
+00000e50: 7272 0c00 0000 5a04 766d 7265 5a04 766d  rr....Z.vmreZ.vm
+00000e60: 7268 7216 0000 0072 1700 0000 7218 0000  rhr....r....r...
+00000e70: 005a 106e 756d 6265 725f 6465 6e73 6974  .Z.number_densit
+00000e80: 795f 655a 106e 756d 6265 725f 6465 6e73  y_eZ.number_dens
+00000e90: 6974 795f 6872 1900 0000 721a 0000 005a  ity_hr....r....Z
+00000ea0: 066c 6f67 6162 635a 0564 7461 7568 720e  .logabcZ.dtauhr.
+00000eb0: 0000 0072 0e00 0000 720f 0000 00da 1a6c  ...r....r......l
+00000ec0: 6179 6572 5f6f 7074 6963 616c 5f64 6570  ayer_optical_dep
+00000ed0: 7468 5f48 6d69 6e75 7358 0000 0073 2400  th_HminusX...s$.
+00000ee0: 0000 0011 0a01 0801 0801 0a01 0801 0801  ................
+00000ef0: 02ff 0402 0c01 02ff 0401 0eff 0201 02ff  ................
+00000f00: 0201 0eff 0403 721f 0000 0029 17da 075f  ......r....)..._
+00000f10: 5f64 6f63 5f5f 5a03 6a61 7872 0200 0000  _doc__Z.jaxr....
+00000f20: 7203 0000 005a 096a 6178 2e6e 756d 7079  r....Z.jax.numpy
+00000f30: da05 6e75 6d70 7972 1200 0000 5a15 6578  ..numpyr....Z.ex
+00000f40: 6f6a 6178 2e73 7065 632e 6869 7472 616e  ojax.spec.hitran
+00000f50: 6369 6172 0400 0000 5a12 6578 6f6a 6178  ciar....Z.exojax
+00000f60: 2e73 7065 632e 686d 696e 7573 7205 0000  .spec.hminusr...
+00000f70: 005a 1365 786f 6a61 782e 6174 6d2e 6964  .Z.exojax.atm.id
+00000f80: 6561 6c67 6173 7206 0000 005a 1665 786f  ealgasr....Z.exo
+00000f90: 6a61 782e 7574 696c 732e 636f 6e73 7461  jax.utils.consta
+00000fa0: 6e74 7372 0700 0000 7208 0000 0072 0a00  ntsr....r....r..
+00000fb0: 0000 5a15 6578 6f6a 6178 2e73 7065 632e  ..Z.exojax.spec.
+00000fc0: 6474 6175 5f6d 6d77 6c72 0b00 0000 7210  dtau_mmwlr....r.
+00000fd0: 0000 0072 1b00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000fe0: 0000 720e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
+00000ff0: 0072 0f00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001000: 0100 0000 7318 0000 0004 0410 010c 010c  ....s...........
+00001010: 010c 010c 0110 010c 010c 0308 1508 2108  ..............!.
+00001020: 13                                       .
```

## exojax/spec/__pycache__/lpf.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 12592 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 3031 0000  U.......!..d01..
+00000000: 550d 0d0a 0000 0000 e566 1664 3031 0000  U........f.d01..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2001 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c07 6d08 5a08 6d09 5a09 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c07 6d0a 5a0a 0100 6401 6406 6c01  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

## exojax/spec/__pycache__/make_numatrix.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Feb  6 13:31:25 2023 UTC, .py size: 3836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2d01 e163 fc0e 0000  U.......-..c....
+00000000: 550d 0d0a 0000 0000 f75d 7864 fc0e 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6400 6402 6c03 5a05 6400  m.Z...d.d.l.Z.d.
 00000050: 6402 6c06 5a06 641c 6404 6405 8401 5a07  d.l.Z.d.d.d...Z.
 00000060: 641d 6407 6408 8401 5a08 6501 6409 640a  d.d.d...Z.e.d.d.
 00000070: 8400 8301 5a09 6501 640b 640c 8400 8301  ....Z.e.d.d.....
```

## exojax/spec/__pycache__/modit.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 25279 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 bf62 0000  U.......!..d.b..
+00000000: 550d 0d0a 0000 0000 e566 1664 bf62 0000  U........f.d.b..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7401 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 6d02 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

## exojax/spec/__pycache__/modit_scanfft.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Feb 13 02:26:04 2023 UTC, .py size: 5095 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bc9f e963 e713 0000  U..........c....
+00000000: 550d 0d0a 0000 0000 28c3 2864 e713 0000  U.......(.(d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 6d06 5a06 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6401 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 8400 5a0d 6505 6409 640a  ..d.d...Z.e.d.d.
```

## exojax/spec/__pycache__/opacalc.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 19215 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 0f4b 0000  U.......!..d.K..
+00000000: 550d 0d0a 0000 0000 f75d 7864 0f4b 0000  U........]xd.K..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6403 6703 5a01 6404 6405  Z.d.d.d.g.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6404 6406 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 6404 6407 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000060: 6404 6408 6c08 6d09 5a09 0100 6404 6409  d.d.l.m.Z...d.d.
 00000070: 6c06 6d0a 5a0a 0100 6404 640a 6c08 6d0b  l.m.Z...d.d.l.m.
```

## exojax/spec/__pycache__/opachord.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Mar 11 21:51:55 2023 UTC, .py size: 1248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,88 +1,113 @@
-00000000: 550d 0d0a 0000 0000 fbf7 0c64 e004 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 9c57 2d64 8406 0000  U........W-d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c01  d.l.m.Z...d.d.l.
 00000040: 5a03 6400 6402 6c04 6d05 5a05 0100 6505  Z.d.d.l.m.Z...e.
 00000050: 6403 6404 8400 8301 5a06 6405 6406 8400  d.d.....Z.d.d...
 00000060: 5a07 6401 5300 2907 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da03 6a69 7463 0200 0000 0000 0000 0000  ..jitc..........
-00000080: 0000 0600 0000 0600 0000 4300 0000 73a8  ..........C...s.
-00000090: 0000 0074 00a0 017c 0164 01a1 027d 027c  ...t...|.d...}.|
-000000a0: 026a 0264 0219 00a0 037c 0164 0219 00a1  .j.d.....|.d....
-000000b0: 017d 027c 006a 0264 0219 00a0 0374 006a  .}.|.j.d.....t.j
-000000c0: 04a1 017d 0074 00a0 057c 0164 0364 0364  ...}.t...|.d.d.d
-000000d0: 0385 0266 0219 0064 0413 007c 0164 0364  ...f...d...|.d.d
-000000e0: 0385 0264 0366 0219 0064 0413 0018 00a1  ...d.f...d......
-000000f0: 017d 0374 00a0 057c 0264 0364 0364 0385  .}.t...|.d.d.d..
-00000100: 0266 0219 0064 0413 007c 0164 0364 0385  .f...d...|.d.d..
-00000110: 0264 0366 0219 0064 0413 0018 00a1 017d  .d.f...d.......}
-00000120: 0464 057c 047c 0318 0014 007c 001b 007d  .d.|.|.....|...}
-00000130: 0574 00a0 067c 05a1 0153 0029 0661 2801  .t...|...S.).a(.
-00000140: 0000 636f 6d70 7574 6520 6368 6f72 6420  ..compute chord 
-00000150: 6765 6f6d 6574 7269 6320 6d61 7472 6978  geometric matrix
-00000160: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00000170: 2020 2020 6865 6967 6874 2028 3144 2061      height (1D a
-00000180: 7272 6179 293a 2028 6e6f 726d 616c 697a  rray): (normaliz
-00000190: 6564 2920 6865 6967 6874 206f 6620 7468  ed) height of th
-000001a0: 6520 6c61 7965 7273 2066 726f 6d20 746f  e layers from to
-000001b0: 7020 6174 6d6f 7370 6865 7265 2c20 4e6c  p atmosphere, Nl
-000001c0: 6179 6572 0a20 2020 2020 2020 2072 6164  ayer.        rad
-000001d0: 6975 7320 2831 4420 6172 7261 7929 3a20  ius (1D array): 
+00000080: 0000 0700 0000 0600 0000 4300 0000 73a2  ..........C...s.
+00000090: 0000 007c 0164 0119 007c 0064 0119 0017  ...|.d...|.d....
+000000a0: 007d 0274 00a0 017c 0164 02a1 027d 037c  .}.t...|.d...}.|
+000000b0: 036a 0264 0119 00a0 037c 02a1 017d 0374  .j.d.....|...}.t
+000000c0: 00a0 047c 0164 0364 0364 0385 0266 0219  ...|.d.d.d...f..
+000000d0: 0064 0413 007c 0164 0364 0385 0264 0366  .d...|.d.d...d.f
+000000e0: 0219 0064 0413 0018 00a1 017d 0474 00a0  ...d.......}.t..
+000000f0: 047c 0364 0364 0364 0385 0266 0219 0064  .|.d.d.d...f...d
+00000100: 0413 007c 0164 0364 0385 0264 0366 0219  ...|.d.d...d.f..
+00000110: 0064 0413 0018 00a1 017d 0564 057c 057c  .d.......}.d.|.|
+00000120: 0418 0014 007c 001b 007d 0674 00a0 057c  .....|...}.t...|
+00000130: 06a1 0153 0029 0661 8802 0000 636f 6d70  ...S.).a....comp
+00000140: 7574 6520 6368 6f72 6420 6765 6f6d 6574  ute chord geomet
+00000150: 7269 6320 6d61 7472 6978 0a0a 2020 2020  ric matrix..    
+00000160: 4172 6773 3a0a 2020 2020 2020 2020 6865  Args:.        he
+00000170: 6967 6874 2028 3144 2061 7272 6179 293a  ight (1D array):
+00000180: 2028 6e6f 726d 616c 697a 6564 2920 6865   (normalized) he
+00000190: 6967 6874 206f 6620 7468 6520 6c61 7965  ight of the laye
+000001a0: 7273 2066 726f 6d20 746f 7020 6174 6d6f  rs from top atmo
+000001b0: 7370 6865 7265 2c20 4e6c 6179 6572 0a20  sphere, Nlayer. 
+000001c0: 2020 2020 2020 2072 6164 6975 735f 6c6f         radius_lo
+000001d0: 7765 7220 2831 4420 6172 7261 7929 3a20  wer (1D array): 
 000001e0: 286e 6f72 6d61 6c69 7a65 6429 2072 6164  (normalized) rad
-000001f0: 6975 7320 6f66 2074 6865 206c 6179 6572  ius of the layer
-00000200: 7320 6672 6f6d 2074 6f70 2061 746d 6f73  s from top atmos
-00000210: 7068 6572 652c 204e 6c61 7965 720a 0a20  phere, Nlayer.. 
-00000220: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00000230: 2020 2020 3244 2061 7272 6179 3a20 6368      2D array: ch
-00000240: 6f72 6420 6765 6f6d 6574 7269 6320 6d61  ord geometric ma
-00000250: 7472 6978 2028 4e6c 6179 6572 2c20 4e6c  trix (Nlayer, Nl
-00000260: 6179 6572 290a 2020 2020 e901 0000 0072  ayer).    .....r
-00000270: 0100 0000 4ee9 0200 0000 6700 0000 0000  ....N.....g.....
-00000280: 0000 4029 07da 036a 6e70 5a04 726f 6c6c  ..@)...jnpZ.roll
-00000290: da02 6174 da03 7365 74da 0369 6e66 da04  ..at..set..inf..
-000002a0: 7371 7274 5a04 7472 696c 2906 da06 6865  sqrtZ.tril)...he
-000002b0: 6967 6874 5a06 7261 6469 7573 5a0b 7261  ightZ.radiusZ.ra
-000002c0: 6469 7573 5f72 6f6c 6c5a 0966 6163 5f72  dius_rollZ.fac_r
-000002d0: 6967 6874 5a08 6661 635f 6c65 6674 5a0a  ightZ.fac_leftZ.
-000002e0: 7261 775f 6d61 7472 6978 a900 720b 0000  raw_matrix..r...
-000002f0: 00fa 3462 7569 6c64 2f62 6469 7374 2e6c  ..4build/bdist.l
-00000300: 696e 7578 2d78 3836 5f36 342f 6567 672f  inux-x86_64/egg/
-00000310: 6578 6f6a 6178 2f73 7065 632f 6f70 6163  exojax/spec/opac
-00000320: 686f 7264 2e70 79da 1663 686f 7264 5f67  hord.py..chord_g
-00000330: 656f 6d65 7472 6963 5f6d 6174 7269 7806  eometric_matrix.
-00000340: 0000 0073 0e00 0000 000b 0c03 1401 1202  ...s............
-00000350: 2e01 2e01 1001 720d 0000 0063 0200 0000  ......r....c....
-00000360: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000370: 4300 0000 730c 0000 0074 00a0 017c 007c  C...s....t...|.|
-00000380: 01a1 0253 0029 0161 3f01 0000 6368 6f72  ...S.).a?...chor
-00000390: 6420 6f70 6163 6974 7920 7665 6374 6f72  d opacity vector
-000003a0: 2066 726f 6d20 6120 6368 6f72 6420 6765   from a chord ge
-000003b0: 6f6d 6574 7269 6320 6d61 7472 6978 2061  ometric matrix a
-000003c0: 6e64 2078 736d 6174 7269 780a 2020 2020  nd xsmatrix.    
-000003d0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000003e0: 2020 2063 686f 7264 5f67 656f 6d65 7472     chord_geometr
-000003f0: 6963 5f6d 6174 7269 7820 286a 6e70 2061  ic_matrix (jnp a
-00000400: 7272 6179 293a 2063 686f 7264 2067 656f  rray): chord geo
-00000410: 6d65 7472 6963 206d 6174 7269 7820 284e  metric matrix (N
-00000420: 6c61 7965 722c 204e 6c61 7965 7229 2c20  layer, Nlayer), 
-00000430: 6c6f 7765 7220 7472 6961 6e67 6c65 206d  lower triangle m
-00000440: 6174 7269 7820 0a20 2020 2020 2020 2078  atrix .        x
-00000450: 736d 6174 7269 7820 286a 6e70 2061 7272  smatrix (jnp arr
-00000460: 6179 293a 2063 726f 7373 2073 6563 7469  ay): cross secti
-00000470: 6f6e 206d 6174 7269 7820 284e 6c61 7965  on matrix (Nlaye
-00000480: 722c 204e 5f77 6176 656e 756d 6265 7229  r, N_wavenumber)
-00000490: 0a0a 2020 2020 5265 7475 726e 733a 2074  ..    Returns: t
-000004a0: 6175 6368 6f72 6420 6d61 7472 6978 2028  auchord matrix (
-000004b0: 4e6c 6179 6572 2c20 4e5f 7761 7665 6e75  Nlayer, N_wavenu
-000004c0: 6d62 6572 290a 0a20 2020 2029 0272 0500  mber)..    ).r..
-000004d0: 0000 da03 646f 7429 0272 0d00 0000 5a08  ....dot).r....Z.
-000004e0: 7873 6d61 7472 6978 720b 0000 0072 0b00  xsmatrixr....r..
-000004f0: 0000 720c 0000 00da 0874 6175 6368 6f72  ..r......tauchor
-00000500: 641d 0000 0073 0200 0000 000a 720f 0000  d....s......r...
-00000510: 0029 085a 096a 6178 2e6e 756d 7079 da05  .).Z.jax.numpy..
-00000520: 6e75 6d70 7972 0500 0000 da02 6e70 5a03  numpyr......npZ.
-00000530: 6a61 7872 0200 0000 720d 0000 0072 0f00  jaxr....r....r..
-00000540: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00000550: 0072 0c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000560: 0100 0000 730a 0000 000c 0108 010c 0302  ....s...........
-00000570: 010a 16                                  ...
+000001f0: 6975 7320 6174 2074 6865 206c 6f77 6572  ius at the lower
+00000200: 2062 6f75 6e64 6172 7920 6672 6f6d 2074   boundary from t
+00000210: 6f70 2074 6f20 626f 7474 6f6d 2028 5230  op to bottom (R0
+00000220: 292c 2028 4e6c 6179 6572 290a 0a20 2020  ), (Nlayer)..   
+00000230: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00000240: 2020 3244 2061 7272 6179 3a20 6368 6f72    2D array: chor
+00000250: 6420 6765 6f6d 6574 7269 6320 6d61 7472  d geometric matr
+00000260: 6978 2028 4e6c 6179 6572 2c20 4e6c 6179  ix (Nlayer, Nlay
+00000270: 6572 292c 206c 6f77 6572 2074 7269 616e  er), lower trian
+00000280: 676c 6520 6d61 7472 6978 0a0a 2020 2020  gle matrix..    
+00000290: 4e6f 7465 733a 0a20 2020 2020 2020 204f  Notes:.        O
+000002a0: 7572 2064 6566 696e 6974 696f 6e73 206f  ur definitions o
+000002b0: 6620 7468 6520 7261 6469 7573 5f6c 6f77  f the radius_low
+000002c0: 6572 2061 6e64 2068 6569 6768 7420 2861  er and height (a
+000002d0: 6e64 2072 6164 6975 735f 746f 702c 2069  nd radius_top, i
+000002e0: 6e74 6572 6e61 6c6c 7920 6465 6669 6e65  nternally define
+000002f0: 6429 2061 7265 2061 7320 666f 6c6c 6f77  d) are as follow
+00000300: 733a 0a20 2020 2020 2020 206e 3d30 2c31  s:.        n=0,1
+00000310: 2c2e 2e2e 2c4e 2d31 0a20 2020 2020 2020  ,...,N-1.       
+00000320: 2072 6164 6975 735f 6c6f 7765 725b 4e2d   radius_lower[N-
+00000330: 315d 203d 2072 6164 6975 735f 6274 6d20  1] = radius_btm 
+00000340: 2869 2e65 2e20 5230 2920 2020 200a 2020  (i.e. R0)    .  
+00000350: 2020 2020 2020 7261 6469 7573 5f6c 6f77        radius_low
+00000360: 6572 5b6e 2d31 5d20 3d20 7261 6469 7573  er[n-1] = radius
+00000370: 5f6c 6f77 6572 5b6e 5d20 2b20 6865 6967  _lower[n] + heig
+00000380: 6874 5b6e 5d0a 2020 2020 2020 2020 7261  ht[n].        ra
+00000390: 6469 7573 5f74 6f70 203d 2072 6164 6975  dius_top = radiu
+000003a0: 735f 6c6f 7765 725b 305d 202b 2068 6569  s_lower[0] + hei
+000003b0: 6768 745b 305d 0a20 2020 2020 2020 200a  ght[0].        .
+000003c0: 2020 2020 7201 0000 00e9 0100 0000 4ee9      r.........N.
+000003d0: 0200 0000 6700 0000 0000 0000 4029 06da  ....g.......@)..
+000003e0: 036a 6e70 5a04 726f 6c6c da02 6174 da03  .jnpZ.roll..at..
+000003f0: 7365 74da 0473 7172 745a 0474 7269 6c29  set..sqrtZ.tril)
+00000400: 07da 0668 6569 6768 745a 0c72 6164 6975  ...heightZ.radiu
+00000410: 735f 6c6f 7765 725a 0a72 6164 6975 735f  s_lowerZ.radius_
+00000420: 746f 705a 0e72 6164 6975 735f 7368 6966  topZ.radius_shif
+00000430: 7465 645a 0966 6163 5f72 6967 6874 5a08  tedZ.fac_rightZ.
+00000440: 6661 635f 6c65 6674 5a0a 7261 775f 6d61  fac_leftZ.raw_ma
+00000450: 7472 6978 a900 720a 0000 00fa 3462 7569  trix..r.....4bui
+00000460: 6c64 2f62 6469 7374 2e6c 696e 7578 2d78  ld/bdist.linux-x
+00000470: 3836 5f36 342f 6567 672f 6578 6f6a 6178  86_64/egg/exojax
+00000480: 2f73 7065 632f 6f70 6163 686f 7264 2e70  /spec/opachord.p
+00000490: 79da 1663 686f 7264 5f67 656f 6d65 7472  y..chord_geometr
+000004a0: 6963 5f6d 6174 7269 7806 0000 0073 0e00  ic_matrix....s..
+000004b0: 0000 0013 1001 0c01 1001 2e01 2e01 1001  ................
+000004c0: 720c 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000004d0: 0000 0200 0000 0400 0000 4300 0000 730c  ..........C...s.
+000004e0: 0000 0074 00a0 017c 007c 01a1 0253 0029  ...t...|.|...S.)
+000004f0: 0161 5f01 0000 6368 6f72 6420 6f70 7469  .a_...chord opti
+00000500: 6361 6c20 6465 7074 6820 7665 6374 6f72  cal depth vector
+00000510: 2066 726f 6d20 6120 6368 6f72 6420 6765   from a chord ge
+00000520: 6f6d 6574 7269 6320 6d61 7472 6978 2061  ometric matrix a
+00000530: 6e64 2064 7461 750a 2020 2020 0a20 2020  nd dtau.    .   
+00000540: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
+00000550: 686f 7264 5f67 656f 6d65 7472 6963 5f6d  hord_geometric_m
+00000560: 6174 7269 7820 286a 6e70 2061 7272 6179  atrix (jnp array
+00000570: 293a 2063 686f 7264 2067 656f 6d65 7472  ): chord geometr
+00000580: 6963 206d 6174 7269 7820 284e 6c61 7965  ic matrix (Nlaye
+00000590: 722c 204e 6c61 7965 7229 2c20 6c6f 7765  r, Nlayer), lowe
+000005a0: 7220 7472 6961 6e67 6c65 206d 6174 7269  r triangle matri
+000005b0: 7820 0a20 2020 2020 2020 2064 7461 7520  x .        dtau 
+000005c0: 286a 6e70 2061 7272 6179 293a 206c 6179  (jnp array): lay
+000005d0: 6572 206f 7074 6963 616c 2064 6570 7468  er optical depth
+000005e0: 206d 6174 7269 782c 2064 7461 7520 284e   matrix, dtau (N
+000005f0: 6c61 7965 722c 204e 5f77 6176 656e 756d  layer, N_wavenum
+00000600: 6265 7229 0a0a 2020 2020 5265 7475 726e  ber)..    Return
+00000610: 733a 2063 686f 7264 206f 7074 6963 616c  s: chord optical
+00000620: 2064 6570 7468 2028 7461 7563 686f 7264   depth (tauchord
+00000630: 2920 6d61 7472 6978 2028 4e6c 6179 6572  ) matrix (Nlayer
+00000640: 2c20 4e5f 7761 7665 6e75 6d62 6572 290a  , N_wavenumber).
+00000650: 0a20 2020 2029 0272 0500 0000 da03 646f  .    ).r......do
+00000660: 7429 0272 0c00 0000 5a04 6474 6175 720a  t).r....Z.dtaur.
+00000670: 0000 0072 0a00 0000 720b 0000 00da 1363  ...r....r......c
+00000680: 686f 7264 5f6f 7074 6963 616c 5f64 6570  hord_optical_dep
+00000690: 7468 2200 0000 7302 0000 0000 0a72 0e00  th"...s......r..
+000006a0: 0000 2908 5a09 6a61 782e 6e75 6d70 79da  ..).Z.jax.numpy.
+000006b0: 056e 756d 7079 7205 0000 00da 026e 705a  .numpyr......npZ
+000006c0: 036a 6178 7202 0000 0072 0c00 0000 720e  .jaxr....r....r.
+000006d0: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+000006e0: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000006f0: 3e01 0000 0073 0a00 0000 0c01 0801 0c03  >....s..........
+00000700: 0201 0a1b                                ....
```

## exojax/spec/__pycache__/optgrid.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 3438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 6e0d 0000  U.......!..dn...
+00000000: 550d 0d0a 0000 0000 f75d 7864 6e0d 0000  U........]xdn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0a 6d0a 5a0a 0100 640e  ..d.d.l.m.Z...d.
```

## exojax/spec/__pycache__/premodit.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 22792 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 0859 0000  U.......!..d.Y..
+00000000: 550d 0d0a 0000 0000 f75d 7864 0859 0000  U........]xd.Y..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e01 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d01 5a04 0100 6401 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0b 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

## exojax/spec/__pycache__/response.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 3364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 240d 0000  U.......!..d$...
+00000000: 550d 0d0a 0000 0000 f75d 7864 240d 0000  U........]xd$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6401 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6401 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6401 6407 6c0c  d.l.m.Z...d.d.l.
```

## exojax/spec/__pycache__/rtransfer.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 10477 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 ed28 0000  U.......!..d.(..
+00000000: 550d 0d0a 0000 0000 f75d 7864 ed28 0000  U........]xd.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6403 6c05 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

## exojax/spec/__pycache__/set_ditgrid.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Dec  7 12:18:00 2022 UTC, .py size: 5466 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7884 9063 5a15 0000  U.......x..cZ...
+00000000: 550d 0d0a 0000 0000 fd5d 7864 5b15 0000  U........]xd[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 640f 6405 6406 8401 5a04 6410 6407  Z.d.d.d...Z.d.d.
 00000050: 6408 8401 5a05 6411 6409 640a 8401 5a06  d...Z.d.d.d...Z.
 00000060: 6412 640b 640c 8401 5a07 6413 640d 640e  d.d.d...Z.d.d.d.
 00000070: 8401 5a08 6402 5300 2914 7a5d 7365 7420  ..Z.d.S.).z]set 
@@ -48,277 +48,271 @@
 000002f0: 2020 2020 2020 496e 2074 6869 7320 6361        In this ca
 00000300: 7365 2c20 7468 6520 6772 6964 2077 6964  se, the grid wid
 00000310: 7468 2064 6f65 7320 6e6f 7420 6e65 6564  th does not need
 00000320: 2074 6f20 6265 2064 6974 5f67 7269 645f   to be dit_grid_
 00000330: 7265 736f 6c75 7469 6f6e 2065 7861 6374  resolution exact
 00000340: 6c79 2e0a 0a20 2020 2052 6574 7572 6e73  ly...    Returns
 00000350: 3a0a 2020 2020 2020 2020 6772 6964 2066  :.        grid f
-00000360: 6f72 2044 4954 0a20 2020 20e7 0000 0000  or DIT.    .....
+00000360: 6f72 2044 4954 0a20 2020 2067 0000 0000  or DIT.    g....
 00000370: 0000 0000 7a4a 5468 6572 6520 6578 6973  ....zJThere exis
 00000380: 7473 206e 6567 6174 6976 6520 6f72 207a  ts negative or z
 00000390: 6572 6f20 6761 6d6d 612e 204d 4f44 4954  ero gamma. MODIT
 000003a0: 2f44 4954 2064 6f65 7320 6e6f 7420 7375  /DIT does not su
 000003b0: 7070 6f72 7420 7468 6973 2063 6173 652e  pport this case.
 000003c0: a901 da05 6474 7970 65e9 0200 0000 46e9  ....dtype.....F.
 000003d0: 0100 0000 290b da02 6e70 da03 6d69 6eda  ....)...np..min.
 000003e0: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
 000003f0: 036c 6f67 da03 6d61 78da 096e 6578 7461  .log..max..nexta
-00000400: 6674 6572 da03 696e 6672 0500 0000 da03  fter..infr......
+00000400: 6674 6572 da03 696e 6672 0400 0000 da03  fter..infr......
 00000410: 696e 74da 0365 7870 da08 6c69 6e73 7061  int..exp..linspa
 00000420: 6365 2908 da0e 696e 7075 745f 7661 7269  ce)...input_vari
 00000430: 6162 6c65 da13 6469 745f 6772 6964 5f72  able..dit_grid_r
 00000440: 6573 6f6c 7574 696f 6eda 0561 646f 7074  esolution..adopt
 00000450: da05 6c78 6d69 6eda 056c 786d 6178 da04  ..lxmin..lxmax..
 00000460: 646c 6f67 da02 4e67 da04 6772 6964 a900  dlog..Ng..grid..
-00000470: 721a 0000 00fa 3762 7569 6c64 2f62 6469  r.....7build/bdi
+00000470: 7219 0000 00fa 3762 7569 6c64 2f62 6469  r.....7build/bdi
 00000480: 7374 2e6c 696e 7578 2d78 3836 5f36 342f  st.linux-x86_64/
 00000490: 6567 672f 6578 6f6a 6178 2f73 7065 632f  egg/exojax/spec/
 000004a0: 7365 745f 6469 7467 7269 642e 7079 da14  set_ditgrid.py..
 000004b0: 6469 7467 7269 645f 6c6f 675f 696e 7465  ditgrid_log_inte
 000004c0: 7276 616c 0a00 0000 7314 0000 0000 0c16  rval....s.......
 000004d0: 0210 0110 0114 0108 0110 0108 0122 0214  ............."..
-000004e0: 0172 1c00 0000 6304 0000 0000 0000 0000  .r....c.........
+000004e0: 0172 1b00 0000 6304 0000 0000 0000 0000  .r....c.........
 000004f0: 0000 0009 0000 0006 0000 0043 0000 0073  ...........C...s
-00000500: a800 0000 7c02 6401 6b08 720c 6402 7d02  ....|.d.k.r.d.}.
-00000510: 7400 a001 7c02 7c00 1400 a101 6403 6b04  t...|.|.....d.k.
-00000520: 7326 7402 6404 8301 8201 7400 a001 7c02  s&t.d.....t...|.
-00000530: 7c00 1400 a101 7d04 7400 a003 7c02 7c00  |.....}.t...|.|.
-00000540: 1400 a101 7d05 7400 6a04 7c05 7400 6a05  ....}.t.j.|.t.j.
-00000550: 7c05 6a06 6405 8d03 7d05 7c05 7c04 1800  |.j.d...}.|.|...
-00000560: 7d06 7407 7c06 7c01 1b00 8301 6406 1700  }.t.|.|.....d...
-00000570: 7d07 7c03 6407 6b02 7292 7400 a008 7c04  }.|.d.k.r.t...|.
-00000580: 7c04 7c07 6408 1800 7c01 1400 1700 7c07  |.|.d...|.....|.
-00000590: a103 7d08 6e0e 7400 a008 7c04 7c05 7c07  ..}.n.t...|.|.|.
-000005a0: a103 7d08 7c08 7c02 1b00 5300 2909 6109  ..}.|.|...S.).a.
-000005b0: 0200 0067 656e 6572 6174 6520 4449 5420  ...generate DIT 
-000005c0: 4752 4944 2077 6974 6820 636f 6e73 7461  GRID with consta
-000005d0: 6e74 2069 6e74 6572 7661 6c20 696e 206c  nt interval in l
-000005e0: 696e 6561 7220 7363 616c 650a 0a20 2020  inear scale..   
-000005f0: 2041 7267 733a 0a20 2020 2020 2020 2069   Args:.        i
-00000600: 6e70 7574 5f76 6172 6961 626c 653a 2069  nput_variable: i
-00000610: 6e70 7574 2061 7272 6179 2c20 652e 672e  nput array, e.g.
-00000620: 206e 5f54 6578 7020 2874 656d 7065 7261   n_Texp (tempera
-00000630: 7475 7265 2065 7870 6f6e 656e 7429 2061  ture exponent) a
-00000640: 7272 6179 2028 4e6c 696e 6529 0a20 2020  rray (Nline).   
-00000650: 2020 2020 2064 6974 5f67 7269 645f 7265       dit_grid_re
-00000660: 736f 6c75 7469 6f6e 3a20 6772 6964 2072  solution: grid r
-00000670: 6573 6f6c 7574 696f 6e2e 2064 6974 5f67  esolution. dit_g
-00000680: 7269 645f 7265 736f 6c75 7469 6f6e 3d30  rid_resolution=0
-00000690: 2e31 2028 6465 6661 7574 2920 6d65 616e  .1 (defaut) mean
-000006a0: 7320 6120 6772 6964 2070 6f69 6e74 2070  s a grid point p
-000006b0: 6572 2064 6967 6974 0a20 2020 2020 2020  er digit.       
-000006c0: 2077 6569 6768 743a 2077 6569 6768 742c   weight: weight,
-000006d0: 2065 2e67 2e20 6e70 2e61 6273 286c 6e28   e.g. np.abs(ln(
-000006e0: 5429 2d6c 6e28 5472 6566 2929 0a20 2020  T)-ln(Tref)).   
-000006f0: 2020 2020 2061 646f 7074 3a20 6966 2054       adopt: if T
-00000700: 7275 652c 206d 696e 2c20 6d61 7820 6772  rue, min, max gr
-00000710: 6964 2070 6f69 6e74 7320 6172 6520 7573  id points are us
-00000720: 6564 2061 7420 6d69 6e20 616e 6420 6d61  ed at min and ma
-00000730: 7820 7661 6c75 6573 206f 6620 782e 0a20  x values of x.. 
-00000740: 2020 2020 2020 2049 6e20 7468 6973 2063         In this c
-00000750: 6173 652c 2074 6865 2067 7269 6420 7769  ase, the grid wi
-00000760: 6474 6820 646f 6573 206e 6f74 206e 6565  dth does not nee
-00000770: 6420 746f 2062 6520 6469 745f 6772 6964  d to be dit_grid
-00000780: 5f72 6573 6f6c 7574 696f 6e20 6578 6163  _resolution exac
-00000790: 746c 792e 0a0a 2020 2020 5265 7475 726e  tly...    Return
-000007a0: 733a 0a20 2020 2020 2020 2067 7269 6420  s:.        grid 
-000007b0: 666f 7220 4449 540a 2020 2020 4e67 0000  for DIT.    Ng..
-000007c0: 0000 0000 f03f 7203 0000 007a 3c54 6865  .....?r....z<The
-000007d0: 7265 2065 7869 7374 7320 6e65 6761 7469  re exists negati
-000007e0: 7665 206f 7220 7a65 726f 2076 616c 7565  ve or zero value
-000007f0: 2e20 436f 6e73 6964 6572 2074 6f20 7573  . Consider to us
-00000800: 6520 6e70 2e61 6273 2e72 0400 0000 7206  e np.abs.r....r.
-00000810: 0000 0046 7207 0000 0029 0972 0800 0000  ...Fr....).r....
-00000820: 7209 0000 0072 0a00 0000 720c 0000 0072  r....r....r....r
-00000830: 0d00 0000 720e 0000 0072 0500 0000 720f  ....r....r....r.
-00000840: 0000 0072 1100 0000 2909 7212 0000 0072  ...r....).r....r
-00000850: 1300 0000 da06 7765 6967 6874 7214 0000  ......weightr...
-00000860: 005a 0577 786d 696e 5a05 7778 6d61 785a  .Z.wxminZ.wxmaxZ
-00000870: 0364 7778 7218 0000 0072 1900 0000 721a  .dwxr....r....r.
-00000880: 0000 0072 1a00 0000 721b 0000 00da 1764  ...r....r......d
-00000890: 6974 6772 6964 5f6c 696e 6561 725f 696e  itgrid_linear_in
-000008a0: 7465 7276 616c 2300 0000 7318 0000 0000  terval#...s.....
-000008b0: 0d08 0104 021a 010e 010e 0114 0108 0110  ................
-000008c0: 0108 011c 020e 0172 1e00 0000 6303 0000  .......r....c...
-000008d0: 0000 0000 0000 0000 000d 0000 0009 0000  ................
-000008e0: 0043 0000 0073 e400 0000 7400 a001 7400  .C...s....t...t.
-000008f0: 6a02 7c00 6401 6402 8d02 a101 7d03 7400  j.|.d.d.....}.t.
-00000900: a001 7400 6a03 7c00 6401 6402 8d02 a101  ..t.j.|.d.d.....
-00000910: 7d04 7400 6a04 7c04 7400 6a05 7c04 6a06  }.t.j.|.t.j.|.j.
-00000920: 6403 8d03 7d04 7400 a007 7c04 a101 6404  d...}.t...|...d.
-00000930: 1900 7d05 6700 7d06 7400 a003 7c04 7c03  ..}.g.}.t...|.|.
-00000940: 1800 a101 7d07 7c07 7c01 1b00 a008 7409  ....}.|.|.....t.
-00000950: a101 6405 1700 7d08 740a 6404 7c05 8302  ..d...}.t.d.|...
-00000960: 4400 5d5c 7d09 7c03 7c09 1900 7d0a 7c04  D.]\}.|.|...}.|.
-00000970: 7c09 1900 7d0b 7c02 6406 6b02 72b6 7400  |...}.|.d.k.r.t.
-00000980: a00b 7400 a00c 7c0a 7c0a 7c08 6401 1800  ..t...|.|.|.d...
-00000990: 7c01 1400 1700 7c08 a103 a101 7d0c 6e14  |.....|.....}.n.
-000009a0: 7400 a00b 7400 a00c 7c0a 7c0b 7c08 a103  t...t...|.|.|...
-000009b0: a101 7d0c 7c06 a00d 7c0c a101 0100 7178  ..}.|...|.....qx
-000009c0: 7400 a00e 7c06 a101 7d06 7c06 5300 2907  t...|...}.|.S.).
-000009d0: 6176 0100 0044 4954 2047 5249 4420 4d41  av...DIT GRID MA
-000009e0: 5452 4958 2e0a 0a20 2020 2041 7267 733a  TRIX...    Args:
-000009f0: 0a20 2020 2020 2020 2078 3a20 7369 6d67  .        x: simg
-00000a00: 6144 206f 7220 6761 6d6d 614c 206d 6174  aD or gammaL mat
-00000a10: 7269 7820 284e 6c61 7965 7220 7820 4e6c  rix (Nlayer x Nl
-00000a20: 696e 6529 0a20 2020 2020 2020 2072 6573  ine).        res
-00000a30: 3a20 6772 6964 2072 6573 6f6c 7574 696f  : grid resolutio
-00000a40: 6e2e 2072 6573 3d30 2e31 2028 6465 6661  n. res=0.1 (defa
-00000a50: 7574 2920 6d65 616e 7320 6120 6772 6964  ut) means a grid
-00000a60: 2070 6f69 6e74 2070 6572 2064 6967 6974   point per digit
-00000a70: 0a20 2020 2020 2020 2061 646f 7074 3a20  .        adopt: 
-00000a80: 6966 2054 7275 652c 206d 696e 2c20 6d61  if True, min, ma
-00000a90: 7820 6772 6964 2070 6f69 6e74 7320 6172  x grid points ar
-00000aa0: 6520 7573 6564 2061 7420 6d69 6e20 616e  e used at min an
-00000ab0: 6420 6d61 7820 7661 6c75 6573 206f 6620  d max values of 
-00000ac0: 782e 0a20 2020 2020 2020 2020 2020 2020  x..             
-00000ad0: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
-00000ae0: 7468 6520 6772 6964 2077 6964 7468 2064  the grid width d
-00000af0: 6f65 7320 6e6f 7420 6e65 6564 2074 6f20  oes not need to 
-00000b00: 6265 2072 6573 2065 7861 6374 6c79 2e0a  be res exactly..
-00000b10: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00000b20: 2020 2020 2020 6772 6964 2066 6f72 2044        grid for D
-00000b30: 4954 2028 4e6c 6179 6572 2078 204e 4449  IT (Nlayer x NDI
-00000b40: 5467 7269 6429 0a20 2020 2072 0700 0000  Tgrid).    r....
-00000b50: a901 5a04 6178 6973 7204 0000 0072 0100  ..Z.axisr....r..
-00000b60: 0000 7206 0000 0046 290f 7208 0000 0072  ..r....F).r....r
-00000b70: 0b00 0000 7209 0000 0072 0c00 0000 720d  ....r....r....r.
-00000b80: 0000 0072 0e00 0000 7205 0000 00da 0573  ...r....r......s
-00000b90: 6861 7065 da06 6173 7479 7065 720f 0000  hape..astyper...
-00000ba0: 00da 0572 616e 6765 7210 0000 0072 1100  ...ranger....r..
-00000bb0: 0000 da06 6170 7065 6e64 da05 6172 7261  ....append..arra
-00000bc0: 7929 0dda 0178 da03 7265 7372 1400 0000  y)...x..resr....
-00000bd0: da04 6d6d 696e da04 6d6d 6178 da06 4e6c  ..mmin..mmax..Nl
-00000be0: 6179 6572 da02 676d 7217 0000 0072 1800  ayer..gmr....r..
-00000bf0: 0000 da01 6972 1500 0000 7216 0000 0072  ....ir....r....r
-00000c00: 1900 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
-00000c10: 0000 00da 0e64 6974 6772 6964 5f6d 6174  .....ditgrid_mat
-00000c20: 7269 7840 0000 0073 2000 0000 000c 1401  rix@...s .......
-00000c30: 1401 1402 0e01 0401 0e01 1201 0e01 0801  ................
-00000c40: 0801 0801 2202 1401 0c01 0a01 722c 0000  ....".......r,..
-00000c50: 0063 0300 0000 0000 0000 0000 0000 0d00  .c..............
-00000c60: 0000 0400 0000 4300 0000 739a 0000 0074  ......C...s....t
-00000c70: 006a 0174 00a0 027c 00a1 0164 0164 028d  .j.t...|...d.d..
-00000c80: 027d 0374 006a 0374 00a0 027c 00a1 0164  .}.t.j.t...|...d
-00000c90: 0164 028d 027d 0474 00a0 047c 03a1 0164  .d...}.t...|...d
-00000ca0: 0319 007d 0567 007d 0674 00a0 017c 037c  ...}.g.}.t...|.|
-00000cb0: 0418 00a1 017d 077c 077c 011b 00a0 0574  .....}.|.|.....t
-00000cc0: 06a1 0164 0417 007d 0874 0764 037c 0583  ...d...}.t.d.|..
-00000cd0: 0244 005d 267d 097c 047c 0919 007d 0a7c  .D.]&}.|.|...}.|
-00000ce0: 037c 0919 007d 0b7c 0a7c 0b67 027d 0c7c  .|...}.|.|.g.}.|
-00000cf0: 06a0 087c 0ca1 0101 0071 6474 00a0 097c  ...|.....qdt...|
-00000d00: 06a1 017d 067c 0653 0029 0561 a901 0000  ...}.|.S.).a....
-00000d10: 636f 6d70 7574 6520 4d49 4e20 616e 6420  compute MIN and 
-00000d20: 4d41 5820 4449 5420 4752 4944 204d 4154  MAX DIT GRID MAT
-00000d30: 5249 582e 0a0a 2020 2020 4172 6773 3a0a  RIX...    Args:.
-00000d40: 2020 2020 2020 2020 783a 2067 616d 6d61          x: gamma
-00000d50: 4c20 6d61 7472 6978 2028 4e6c 6179 6572  L matrix (Nlayer
-00000d60: 2078 204e 6c69 6e65 290a 2020 2020 2020   x Nline).      
-00000d70: 2020 6469 745f 6772 6964 5f72 6573 6f6c    dit_grid_resol
-00000d80: 7574 696f 6e3a 2067 7269 6420 7265 736f  ution: grid reso
-00000d90: 6c75 7469 6f6e 2e20 6469 745f 6772 6964  lution. dit_grid
-00000da0: 5f72 6573 6f6c 7574 696f 6e3d 302e 3120  _resolution=0.1 
-00000db0: 2864 6566 6175 7429 206d 6561 6e73 2061  (defaut) means a
-00000dc0: 2067 7269 6420 706f 696e 7420 7065 7220   grid point per 
-00000dd0: 6469 6769 740a 2020 2020 2020 2020 6164  digit.        ad
-00000de0: 6f70 743a 2069 6620 5472 7565 2c20 6d69  opt: if True, mi
-00000df0: 6e2c 206d 6178 2067 7269 6420 706f 696e  n, max grid poin
-00000e00: 7473 2061 7265 2075 7365 6420 6174 206d  ts are used at m
-00000e10: 696e 2061 6e64 206d 6178 2076 616c 7565  in and max value
-00000e20: 7320 6f66 2078 2e20 496e 2074 6869 7320  s of x. In this 
-00000e30: 6361 7365 2c20 7468 6520 6772 6964 2077  case, the grid w
-00000e40: 6964 7468 2064 6f65 7320 6e6f 7420 6e65  idth does not ne
-00000e50: 6564 2074 6f20 6265 2064 6974 5f67 7269  ed to be dit_gri
-00000e60: 645f 7265 736f 6c75 7469 6f6e 2065 7861  d_resolution exa
-00000e70: 6374 6c79 2e0a 0a20 2020 2052 6574 7572  ctly...    Retur
-00000e80: 6e73 3a0a 2020 2020 2020 2020 6d69 6e69  ns:.        mini
-00000e90: 6d75 6d20 616e 6420 6d61 7869 6d75 6d20  mum and maximum 
-00000ea0: 666f 7220 4449 5420 2864 676d 5f6d 696e  for DIT (dgm_min
-00000eb0: 6d61 7829 0a20 2020 2072 0700 0000 721f  max).    r....r.
-00000ec0: 0000 0072 0100 0000 7206 0000 0029 0a72  ...r....r....).r
-00000ed0: 0800 0000 720c 0000 00da 056c 6f67 3130  ....r......log10
-00000ee0: 7209 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00000ef0: 0f00 0000 7222 0000 0072 2300 0000 7224  ....r"...r#...r$
-00000f00: 0000 0029 0d72 2500 0000 7213 0000 0072  ...).r%...r....r
-00000f10: 1400 0000 7228 0000 0072 2700 0000 7229  ....r(...r'...r)
-00000f20: 0000 005a 0a64 676d 5f6d 696e 6d61 7872  ...Z.dgm_minmaxr
-00000f30: 1700 0000 7218 0000 0072 2b00 0000 7215  ....r....r+...r.
-00000f40: 0000 0072 1600 0000 7219 0000 0072 1a00  ...r....r....r..
-00000f50: 0000 721a 0000 0072 1b00 0000 da15 6d69  ..r....r......mi
-00000f60: 6e6d 6178 5f64 6974 6772 6964 5f6d 6174  nmax_ditgrid_mat
-00000f70: 7269 7860 0000 0073 1a00 0000 000b 1401  rix`...s........
-00000f80: 1401 0e01 0401 0e01 1201 0e01 0801 0801  ................
-00000f90: 0801 0c01 0a01 722e 0000 0063 0300 0000  ......r....c....
-00000fa0: 0000 0000 0000 0000 0d00 0000 0700 0000  ................
-00000fb0: 4300 0000 73e0 0000 0074 00a0 017c 00a1  C...s....t...|..
-00000fc0: 017d 0074 006a 027c 0064 0164 0185 0264  .}.t.j.|.d.d...d
-00000fd0: 0164 0185 0264 0266 0319 0064 0264 038d  .d...d.f...d.d..
-00000fe0: 027d 0374 006a 037c 0064 0164 0185 0264  .}.t.j.|.d.d...d
-00000ff0: 0164 0185 0264 0466 0319 0064 0264 038d  .d...d.f...d.d..
-00001000: 027d 0474 00a0 037c 047c 0318 00a1 017d  .}.t...|.|.....}
-00001010: 0567 007d 067c 057c 011b 00a0 0474 05a1  .g.}.|.|.....t..
-00001020: 0164 0517 007d 0774 067c 0383 017d 0874  .d...}.t.|...}.t
-00001030: 0764 027c 0883 0244 005d 507d 097c 037c  .d.|...D.]P}.|.|
-00001040: 0919 007d 0a7c 047c 0919 007d 0b7c 0264  ...}.|.|...}.|.d
-00001050: 066b 0272 b874 00a0 087c 0a7c 0a7c 0764  .k.r.t...|.|.|.d
-00001060: 0418 007c 0114 0017 007c 07a1 037d 0c6e  ...|.....|...}.n
-00001070: 0e74 00a0 087c 0a7c 0b7c 07a1 037d 0c7c  .t...|.|.|...}.|
-00001080: 06a0 097c 0ca1 0101 0071 8074 00a0 017c  ...|.....q.t...|
-00001090: 06a1 017d 067c 0653 0029 0761 f901 0000  ...}.|.S.).a....
-000010a0: 5072 6563 6f6d 7075 7469 6e67 204d 4f44  Precomputing MOD
-000010b0: 4954 2047 5249 4420 4d41 5452 4958 2066  IT GRID MATRIX f
-000010c0: 6f72 206e 6f72 6d61 6c69 7a65 6420 4761  or normalized Ga
-000010d0: 6d6d 614c 2e0a 0a20 2020 2041 7267 733a  mmaL...    Args:
-000010e0: 0a20 2020 2020 2020 2073 6574 5f67 6d5f  .        set_gm_
-000010f0: 6d69 6e6d 6178 3a20 7365 7420 6f66 206d  minmax: set of m
-00001100: 696e 6d61 7820 6f66 2064 6974 6772 6964  inmax of ditgrid
-00001110: 206d 6174 7269 7820 666f 7220 6469 6666   matrix for diff
-00001120: 6572 656e 7420 7061 7261 6d65 7465 7273  erent parameters
-00001130: 205b 4e73 616d 706c 652c 204e 6c61 7965   [Nsample, Nlaye
-00001140: 7273 2c20 325d 2c20 323d 6d69 6e2c 6d61  rs, 2], 2=min,ma
-00001150: 780a 2020 2020 2020 2020 6469 745f 6772  x.        dit_gr
-00001160: 6964 5f72 6573 6f6c 7574 696f 6e3a 2067  id_resolution: g
-00001170: 7269 6420 7265 736f 6c75 7469 6f6e 2e20  rid resolution. 
-00001180: 6469 745f 6772 6964 5f72 6573 6f6c 7574  dit_grid_resolut
-00001190: 696f 6e3d 302e 3120 2864 6566 6175 7429  ion=0.1 (defaut)
-000011a0: 206d 6561 6e73 2061 2067 7269 6420 706f   means a grid po
-000011b0: 696e 7420 7065 7220 6469 6769 740a 2020  int per digit.  
-000011c0: 2020 2020 2020 6164 6f70 743a 2069 6620        adopt: if 
-000011d0: 5472 7565 2c20 6d69 6e2c 206d 6178 2067  True, min, max g
-000011e0: 7269 6420 706f 696e 7473 2061 7265 2075  rid points are u
-000011f0: 7365 6420 6174 206d 696e 2061 6e64 206d  sed at min and m
-00001200: 6178 2076 616c 7565 7320 6f66 2078 2e20  ax values of x. 
-00001210: 496e 2074 6869 7320 6361 7365 2c20 7468  In this case, th
-00001220: 6520 6772 6964 2077 6964 7468 2064 6f65  e grid width doe
-00001230: 7320 6e6f 7420 6e65 6564 2074 6f20 6265  s not need to be
-00001240: 2064 6974 5f67 7269 645f 7265 736f 6c75   dit_grid_resolu
-00001250: 7469 6f6e 2065 7861 6374 6c79 2e0a 0a20  tion exactly... 
-00001260: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00001270: 2020 2020 6772 6964 2066 6f72 2044 4954      grid for DIT
-00001280: 2028 4e6c 6179 6572 2078 204e 4449 5467   (Nlayer x NDITg
-00001290: 7269 6429 0a20 2020 204e 7201 0000 0072  rid).    Nr....r
-000012a0: 1f00 0000 7207 0000 0072 0600 0000 4629  ....r....r....F)
-000012b0: 0a72 0800 0000 7224 0000 0072 0900 0000  .r....r$...r....
-000012c0: 720c 0000 0072 2100 0000 720f 0000 00da  r....r!...r.....
-000012d0: 036c 656e 7222 0000 005a 086c 6f67 7370  .lenr"...Z.logsp
-000012e0: 6163 6572 2300 0000 290d 5a0d 7365 745f  acer#...).Z.set_
-000012f0: 676d 5f6d 696e 6d61 7872 1300 0000 7214  gm_minmaxr....r.
-00001300: 0000 005a 096c 6d69 6e61 7272 6179 5a09  ...Z.lminarrayZ.
-00001310: 6c6d 6178 6172 7261 7972 1700 0000 722a  lmaxarrayr....r*
-00001320: 0000 0072 1800 0000 7229 0000 0072 2b00  ...r....r)...r+.
-00001330: 0000 7215 0000 0072 1600 0000 7219 0000  ..r....r....r...
-00001340: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001350: da1f 7072 6563 6f6d 7075 7465 5f6d 6f64  ..precompute_mod
-00001360: 6974 5f64 6974 6772 6964 5f6d 6174 7269  it_ditgrid_matri
-00001370: 7879 0000 0073 2000 0000 000b 0a01 2001  xy...s ....... .
-00001380: 2001 0e01 0401 1201 0801 0e01 0801 0801   ...............
-00001390: 0801 1c02 0e01 0c01 0a01 7230 0000 0029  ..........r0...)
-000013a0: 0272 0200 0000 5429 0372 0200 0000 4e54  .r....T).r....NT
-000013b0: 2902 7202 0000 0054 2902 7202 0000 0054  ).r....T).r....T
-000013c0: 2902 7202 0000 0054 2909 da07 5f5f 646f  ).r....T)...__do
-000013d0: 635f 5fda 056e 756d 7079 7208 0000 00da  c__..numpyr.....
-000013e0: 0877 6172 6e69 6e67 7372 1c00 0000 721e  .warningsr....r.
-000013f0: 0000 0072 2c00 0000 722e 0000 0072 3000  ...r,...r....r0.
-00001400: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
-00001410: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001420: 0100 0000 730e 0000 0004 0608 0108 020a  ....s...........
-00001430: 190a 1d0a 200a 19                        .... ..
+00000500: 8e00 0000 7c02 6401 6b08 720c 6402 7d02  ....|.d.k.r.d.}.
+00000510: 7400 a001 7c02 7c00 1400 a101 7d04 7400  t...|.|.....}.t.
+00000520: a002 7c02 7c00 1400 a101 7d05 7400 6a03  ..|.|.....}.t.j.
+00000530: 7c05 7400 6a04 7c05 6a05 6403 8d03 7d05  |.t.j.|.j.d...}.
+00000540: 7c05 7c04 1800 7d06 7406 7c06 7c01 1b00  |.|...}.t.|.|...
+00000550: 8301 6404 1700 7d07 7c03 6405 6b02 7278  ..d...}.|.d.k.rx
+00000560: 7400 a007 7c04 7c04 7c07 6406 1800 7c01  t...|.|.|.d...|.
+00000570: 1400 1700 7c07 a103 7d08 6e0e 7400 a007  ....|...}.n.t...
+00000580: 7c04 7c05 7c07 a103 7d08 7c08 7c02 1b00  |.|.|...}.|.|...
+00000590: 5300 2907 6109 0200 0067 656e 6572 6174  S.).a....generat
+000005a0: 6520 4449 5420 4752 4944 2077 6974 6820  e DIT GRID with 
+000005b0: 636f 6e73 7461 6e74 2069 6e74 6572 7661  constant interva
+000005c0: 6c20 696e 206c 696e 6561 7220 7363 616c  l in linear scal
+000005d0: 650a 0a20 2020 2041 7267 733a 0a20 2020  e..    Args:.   
+000005e0: 2020 2020 2069 6e70 7574 5f76 6172 6961       input_varia
+000005f0: 626c 653a 2069 6e70 7574 2061 7272 6179  ble: input array
+00000600: 2c20 652e 672e 206e 5f54 6578 7020 2874  , e.g. n_Texp (t
+00000610: 656d 7065 7261 7475 7265 2065 7870 6f6e  emperature expon
+00000620: 656e 7429 2061 7272 6179 2028 4e6c 696e  ent) array (Nlin
+00000630: 6529 0a20 2020 2020 2020 2064 6974 5f67  e).        dit_g
+00000640: 7269 645f 7265 736f 6c75 7469 6f6e 3a20  rid_resolution: 
+00000650: 6772 6964 2072 6573 6f6c 7574 696f 6e2e  grid resolution.
+00000660: 2064 6974 5f67 7269 645f 7265 736f 6c75   dit_grid_resolu
+00000670: 7469 6f6e 3d30 2e31 2028 6465 6661 7574  tion=0.1 (defaut
+00000680: 2920 6d65 616e 7320 6120 6772 6964 2070  ) means a grid p
+00000690: 6f69 6e74 2070 6572 2064 6967 6974 0a20  oint per digit. 
+000006a0: 2020 2020 2020 2077 6569 6768 743a 2077         weight: w
+000006b0: 6569 6768 742c 2065 2e67 2e20 6e70 2e61  eight, e.g. np.a
+000006c0: 6273 286c 6e28 5429 2d6c 6e28 5472 6566  bs(ln(T)-ln(Tref
+000006d0: 2929 0a20 2020 2020 2020 2061 646f 7074  )).        adopt
+000006e0: 3a20 6966 2054 7275 652c 206d 696e 2c20  : if True, min, 
+000006f0: 6d61 7820 6772 6964 2070 6f69 6e74 7320  max grid points 
+00000700: 6172 6520 7573 6564 2061 7420 6d69 6e20  are used at min 
+00000710: 616e 6420 6d61 7820 7661 6c75 6573 206f  and max values o
+00000720: 6620 782e 0a20 2020 2020 2020 2049 6e20  f x..        In 
+00000730: 7468 6973 2063 6173 652c 2074 6865 2067  this case, the g
+00000740: 7269 6420 7769 6474 6820 646f 6573 206e  rid width does n
+00000750: 6f74 206e 6565 6420 746f 2062 6520 6469  ot need to be di
+00000760: 745f 6772 6964 5f72 6573 6f6c 7574 696f  t_grid_resolutio
+00000770: 6e20 6578 6163 746c 792e 0a0a 2020 2020  n exactly...    
+00000780: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000790: 2067 7269 6420 666f 7220 4449 540a 2020   grid for DIT.  
+000007a0: 2020 4e67 0000 0000 0000 f03f 7203 0000    Ng.......?r...
+000007b0: 0072 0500 0000 4672 0600 0000 2908 7207  .r....Fr....).r.
+000007c0: 0000 0072 0800 0000 720b 0000 0072 0c00  ...r....r....r..
+000007d0: 0000 720d 0000 0072 0400 0000 720e 0000  ..r....r....r...
+000007e0: 0072 1000 0000 2909 7211 0000 0072 1200  .r....).r....r..
+000007f0: 0000 da06 7765 6967 6874 7213 0000 005a  ....weightr....Z
+00000800: 0577 786d 696e 5a05 7778 6d61 785a 0364  .wxminZ.wxmaxZ.d
+00000810: 7778 7217 0000 0072 1800 0000 7219 0000  wxr....r....r...
+00000820: 0072 1900 0000 721a 0000 00da 1764 6974  .r....r......dit
+00000830: 6772 6964 5f6c 696e 6561 725f 696e 7465  grid_linear_inte
+00000840: 7276 616c 2300 0000 7316 0000 0000 0d08  rval#...s.......
+00000850: 0104 030e 010e 0114 0108 0110 0108 011c  ................
+00000860: 020e 0172 1d00 0000 6303 0000 0000 0000  ...r....c.......
+00000870: 0000 0000 000d 0000 0009 0000 0043 0000  .............C..
+00000880: 0073 e400 0000 7400 a001 7400 6a02 7c00  .s....t...t.j.|.
+00000890: 6401 6402 8d02 a101 7d03 7400 a001 7400  d.d.....}.t...t.
+000008a0: 6a03 7c00 6401 6402 8d02 a101 7d04 7400  j.|.d.d.....}.t.
+000008b0: 6a04 7c04 7400 6a05 7c04 6a06 6403 8d03  j.|.t.j.|.j.d...
+000008c0: 7d04 7400 a007 7c04 a101 6404 1900 7d05  }.t...|...d...}.
+000008d0: 6700 7d06 7400 a003 7c04 7c03 1800 a101  g.}.t...|.|.....
+000008e0: 7d07 7c07 7c01 1b00 a008 7409 a101 6405  }.|.|.....t...d.
+000008f0: 1700 7d08 740a 6404 7c05 8302 4400 5d5c  ..}.t.d.|...D.]\
+00000900: 7d09 7c03 7c09 1900 7d0a 7c04 7c09 1900  }.|.|...}.|.|...
+00000910: 7d0b 7c02 6406 6b02 72b6 7400 a00b 7400  }.|.d.k.r.t...t.
+00000920: a00c 7c0a 7c0a 7c08 6401 1800 7c01 1400  ..|.|.|.d...|...
+00000930: 1700 7c08 a103 a101 7d0c 6e14 7400 a00b  ..|.....}.n.t...
+00000940: 7400 a00c 7c0a 7c0b 7c08 a103 a101 7d0c  t...|.|.|.....}.
+00000950: 7c06 a00d 7c0c a101 0100 7178 7400 a00e  |...|.....qxt...
+00000960: 7c06 a101 7d06 7c06 5300 2907 6176 0100  |...}.|.S.).av..
+00000970: 0044 4954 2047 5249 4420 4d41 5452 4958  .DIT GRID MATRIX
+00000980: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00000990: 2020 2020 2078 3a20 7369 6d67 6144 206f       x: simgaD o
+000009a0: 7220 6761 6d6d 614c 206d 6174 7269 7820  r gammaL matrix 
+000009b0: 284e 6c61 7965 7220 7820 4e6c 696e 6529  (Nlayer x Nline)
+000009c0: 0a20 2020 2020 2020 2072 6573 3a20 6772  .        res: gr
+000009d0: 6964 2072 6573 6f6c 7574 696f 6e2e 2072  id resolution. r
+000009e0: 6573 3d30 2e31 2028 6465 6661 7574 2920  es=0.1 (defaut) 
+000009f0: 6d65 616e 7320 6120 6772 6964 2070 6f69  means a grid poi
+00000a00: 6e74 2070 6572 2064 6967 6974 0a20 2020  nt per digit.   
+00000a10: 2020 2020 2061 646f 7074 3a20 6966 2054       adopt: if T
+00000a20: 7275 652c 206d 696e 2c20 6d61 7820 6772  rue, min, max gr
+00000a30: 6964 2070 6f69 6e74 7320 6172 6520 7573  id points are us
+00000a40: 6564 2061 7420 6d69 6e20 616e 6420 6d61  ed at min and ma
+00000a50: 7820 7661 6c75 6573 206f 6620 782e 0a20  x values of x.. 
+00000a60: 2020 2020 2020 2020 2020 2020 2020 496e                In
+00000a70: 2074 6869 7320 6361 7365 2c20 7468 6520   this case, the 
+00000a80: 6772 6964 2077 6964 7468 2064 6f65 7320  grid width does 
+00000a90: 6e6f 7420 6e65 6564 2074 6f20 6265 2072  not need to be r
+00000aa0: 6573 2065 7861 6374 6c79 2e0a 0a20 2020  es exactly...   
+00000ab0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00000ac0: 2020 6772 6964 2066 6f72 2044 4954 2028    grid for DIT (
+00000ad0: 4e6c 6179 6572 2078 204e 4449 5467 7269  Nlayer x NDITgri
+00000ae0: 6429 0a20 2020 2072 0600 0000 a901 5a04  d).    r......Z.
+00000af0: 6178 6973 7203 0000 0072 0100 0000 7205  axisr....r....r.
+00000b00: 0000 0046 290f 7207 0000 0072 0a00 0000  ...F).r....r....
+00000b10: 7208 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000b20: 0d00 0000 7204 0000 00da 0573 6861 7065  ....r......shape
+00000b30: da06 6173 7479 7065 720e 0000 00da 0572  ..astyper......r
+00000b40: 616e 6765 720f 0000 0072 1000 0000 da06  anger....r......
+00000b50: 6170 7065 6e64 da05 6172 7261 7929 0dda  append..array)..
+00000b60: 0178 da03 7265 7372 1300 0000 da04 6d6d  .x..resr......mm
+00000b70: 696e da04 6d6d 6178 da06 4e6c 6179 6572  in..mmax..Nlayer
+00000b80: da02 676d 7216 0000 0072 1700 0000 da01  ..gmr....r......
+00000b90: 6972 1400 0000 7215 0000 0072 1800 0000  ir....r....r....
+00000ba0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000bb0: 0e64 6974 6772 6964 5f6d 6174 7269 7840  .ditgrid_matrix@
+00000bc0: 0000 0073 2000 0000 000c 1401 1401 1402  ...s ...........
+00000bd0: 0e01 0401 0e01 1201 0e01 0801 0801 0801  ................
+00000be0: 2202 1401 0c01 0a01 722b 0000 0063 0300  ".......r+...c..
+00000bf0: 0000 0000 0000 0000 0000 0d00 0000 0400  ................
+00000c00: 0000 4300 0000 739a 0000 0074 006a 0174  ..C...s....t.j.t
+00000c10: 00a0 027c 00a1 0164 0164 028d 027d 0374  ...|...d.d...}.t
+00000c20: 006a 0374 00a0 027c 00a1 0164 0164 028d  .j.t...|...d.d..
+00000c30: 027d 0474 00a0 047c 03a1 0164 0319 007d  .}.t...|...d...}
+00000c40: 0567 007d 0674 00a0 017c 037c 0418 00a1  .g.}.t...|.|....
+00000c50: 017d 077c 077c 011b 00a0 0574 06a1 0164  .}.|.|.....t...d
+00000c60: 0417 007d 0874 0764 037c 0583 0244 005d  ...}.t.d.|...D.]
+00000c70: 267d 097c 047c 0919 007d 0a7c 037c 0919  &}.|.|...}.|.|..
+00000c80: 007d 0b7c 0a7c 0b67 027d 0c7c 06a0 087c  .}.|.|.g.}.|...|
+00000c90: 0ca1 0101 0071 6474 00a0 097c 06a1 017d  .....qdt...|...}
+00000ca0: 067c 0653 0029 0561 a901 0000 636f 6d70  .|.S.).a....comp
+00000cb0: 7574 6520 4d49 4e20 616e 6420 4d41 5820  ute MIN and MAX 
+00000cc0: 4449 5420 4752 4944 204d 4154 5249 582e  DIT GRID MATRIX.
+00000cd0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00000ce0: 2020 2020 783a 2067 616d 6d61 4c20 6d61      x: gammaL ma
+00000cf0: 7472 6978 2028 4e6c 6179 6572 2078 204e  trix (Nlayer x N
+00000d00: 6c69 6e65 290a 2020 2020 2020 2020 6469  line).        di
+00000d10: 745f 6772 6964 5f72 6573 6f6c 7574 696f  t_grid_resolutio
+00000d20: 6e3a 2067 7269 6420 7265 736f 6c75 7469  n: grid resoluti
+00000d30: 6f6e 2e20 6469 745f 6772 6964 5f72 6573  on. dit_grid_res
+00000d40: 6f6c 7574 696f 6e3d 302e 3120 2864 6566  olution=0.1 (def
+00000d50: 6175 7429 206d 6561 6e73 2061 2067 7269  aut) means a gri
+00000d60: 6420 706f 696e 7420 7065 7220 6469 6769  d point per digi
+00000d70: 740a 2020 2020 2020 2020 6164 6f70 743a  t.        adopt:
+00000d80: 2069 6620 5472 7565 2c20 6d69 6e2c 206d   if True, min, m
+00000d90: 6178 2067 7269 6420 706f 696e 7473 2061  ax grid points a
+00000da0: 7265 2075 7365 6420 6174 206d 696e 2061  re used at min a
+00000db0: 6e64 206d 6178 2076 616c 7565 7320 6f66  nd max values of
+00000dc0: 2078 2e20 496e 2074 6869 7320 6361 7365   x. In this case
+00000dd0: 2c20 7468 6520 6772 6964 2077 6964 7468  , the grid width
+00000de0: 2064 6f65 7320 6e6f 7420 6e65 6564 2074   does not need t
+00000df0: 6f20 6265 2064 6974 5f67 7269 645f 7265  o be dit_grid_re
+00000e00: 736f 6c75 7469 6f6e 2065 7861 6374 6c79  solution exactly
+00000e10: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
+00000e20: 2020 2020 2020 2020 6d69 6e69 6d75 6d20          minimum 
+00000e30: 616e 6420 6d61 7869 6d75 6d20 666f 7220  and maximum for 
+00000e40: 4449 5420 2864 676d 5f6d 696e 6d61 7829  DIT (dgm_minmax)
+00000e50: 0a20 2020 2072 0600 0000 721e 0000 0072  .    r....r....r
+00000e60: 0100 0000 7205 0000 0029 0a72 0700 0000  ....r....).r....
+00000e70: 720b 0000 00da 056c 6f67 3130 7208 0000  r......log10r...
+00000e80: 0072 1f00 0000 7220 0000 0072 0e00 0000  .r....r ...r....
+00000e90: 7221 0000 0072 2200 0000 7223 0000 0029  r!...r"...r#...)
+00000ea0: 0d72 2400 0000 7212 0000 0072 1300 0000  .r$...r....r....
+00000eb0: 7227 0000 0072 2600 0000 7228 0000 005a  r'...r&...r(...Z
+00000ec0: 0a64 676d 5f6d 696e 6d61 7872 1600 0000  .dgm_minmaxr....
+00000ed0: 7217 0000 0072 2a00 0000 7214 0000 0072  r....r*...r....r
+00000ee0: 1500 0000 7218 0000 0072 1900 0000 7219  ....r....r....r.
+00000ef0: 0000 0072 1a00 0000 da15 6d69 6e6d 6178  ...r......minmax
+00000f00: 5f64 6974 6772 6964 5f6d 6174 7269 7860  _ditgrid_matrix`
+00000f10: 0000 0073 1a00 0000 000b 1401 1401 0e01  ...s............
+00000f20: 0401 0e01 1201 0e01 0801 0801 0801 0c01  ................
+00000f30: 0a01 722d 0000 0063 0300 0000 0000 0000  ..r-...c........
+00000f40: 0000 0000 0d00 0000 0700 0000 4300 0000  ............C...
+00000f50: 73e0 0000 0074 00a0 017c 00a1 017d 0074  s....t...|...}.t
+00000f60: 006a 027c 0064 0164 0185 0264 0164 0185  .j.|.d.d...d.d..
+00000f70: 0264 0266 0319 0064 0264 038d 027d 0374  .d.f...d.d...}.t
+00000f80: 006a 037c 0064 0164 0185 0264 0164 0185  .j.|.d.d...d.d..
+00000f90: 0264 0466 0319 0064 0264 038d 027d 0474  .d.f...d.d...}.t
+00000fa0: 00a0 037c 047c 0318 00a1 017d 0567 007d  ...|.|.....}.g.}
+00000fb0: 067c 057c 011b 00a0 0474 05a1 0164 0517  .|.|.....t...d..
+00000fc0: 007d 0774 067c 0383 017d 0874 0764 027c  .}.t.|...}.t.d.|
+00000fd0: 0883 0244 005d 507d 097c 037c 0919 007d  ...D.]P}.|.|...}
+00000fe0: 0a7c 047c 0919 007d 0b7c 0264 066b 0272  .|.|...}.|.d.k.r
+00000ff0: b874 00a0 087c 0a7c 0a7c 0764 0418 007c  .t...|.|.|.d...|
+00001000: 0114 0017 007c 07a1 037d 0c6e 0e74 00a0  .....|...}.n.t..
+00001010: 087c 0a7c 0b7c 07a1 037d 0c7c 06a0 097c  .|.|.|...}.|...|
+00001020: 0ca1 0101 0071 8074 00a0 017c 06a1 017d  .....q.t...|...}
+00001030: 067c 0653 0029 0761 f901 0000 5072 6563  .|.S.).a....Prec
+00001040: 6f6d 7075 7469 6e67 204d 4f44 4954 2047  omputing MODIT G
+00001050: 5249 4420 4d41 5452 4958 2066 6f72 206e  RID MATRIX for n
+00001060: 6f72 6d61 6c69 7a65 6420 4761 6d6d 614c  ormalized GammaL
+00001070: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00001080: 2020 2020 2073 6574 5f67 6d5f 6d69 6e6d       set_gm_minm
+00001090: 6178 3a20 7365 7420 6f66 206d 696e 6d61  ax: set of minma
+000010a0: 7820 6f66 2064 6974 6772 6964 206d 6174  x of ditgrid mat
+000010b0: 7269 7820 666f 7220 6469 6666 6572 656e  rix for differen
+000010c0: 7420 7061 7261 6d65 7465 7273 205b 4e73  t parameters [Ns
+000010d0: 616d 706c 652c 204e 6c61 7965 7273 2c20  ample, Nlayers, 
+000010e0: 325d 2c20 323d 6d69 6e2c 6d61 780a 2020  2], 2=min,max.  
+000010f0: 2020 2020 2020 6469 745f 6772 6964 5f72        dit_grid_r
+00001100: 6573 6f6c 7574 696f 6e3a 2067 7269 6420  esolution: grid 
+00001110: 7265 736f 6c75 7469 6f6e 2e20 6469 745f  resolution. dit_
+00001120: 6772 6964 5f72 6573 6f6c 7574 696f 6e3d  grid_resolution=
+00001130: 302e 3120 2864 6566 6175 7429 206d 6561  0.1 (defaut) mea
+00001140: 6e73 2061 2067 7269 6420 706f 696e 7420  ns a grid point 
+00001150: 7065 7220 6469 6769 740a 2020 2020 2020  per digit.      
+00001160: 2020 6164 6f70 743a 2069 6620 5472 7565    adopt: if True
+00001170: 2c20 6d69 6e2c 206d 6178 2067 7269 6420  , min, max grid 
+00001180: 706f 696e 7473 2061 7265 2075 7365 6420  points are used 
+00001190: 6174 206d 696e 2061 6e64 206d 6178 2076  at min and max v
+000011a0: 616c 7565 7320 6f66 2078 2e20 496e 2074  alues of x. In t
+000011b0: 6869 7320 6361 7365 2c20 7468 6520 6772  his case, the gr
+000011c0: 6964 2077 6964 7468 2064 6f65 7320 6e6f  id width does no
+000011d0: 7420 6e65 6564 2074 6f20 6265 2064 6974  t need to be dit
+000011e0: 5f67 7269 645f 7265 736f 6c75 7469 6f6e  _grid_resolution
+000011f0: 2065 7861 6374 6c79 2e0a 0a20 2020 2052   exactly...    R
+00001200: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001210: 6772 6964 2066 6f72 2044 4954 2028 4e6c  grid for DIT (Nl
+00001220: 6179 6572 2078 204e 4449 5467 7269 6429  ayer x NDITgrid)
+00001230: 0a20 2020 204e 7201 0000 0072 1e00 0000  .    Nr....r....
+00001240: 7206 0000 0072 0500 0000 4629 0a72 0700  r....r....F).r..
+00001250: 0000 7223 0000 0072 0800 0000 720b 0000  ..r#...r....r...
+00001260: 0072 2000 0000 720e 0000 00da 036c 656e  .r ...r......len
+00001270: 7221 0000 005a 086c 6f67 7370 6163 6572  r!...Z.logspacer
+00001280: 2200 0000 290d 5a0d 7365 745f 676d 5f6d  "...).Z.set_gm_m
+00001290: 696e 6d61 7872 1200 0000 7213 0000 005a  inmaxr....r....Z
+000012a0: 096c 6d69 6e61 7272 6179 5a09 6c6d 6178  .lminarrayZ.lmax
+000012b0: 6172 7261 7972 1600 0000 7229 0000 0072  arrayr....r)...r
+000012c0: 1700 0000 7228 0000 0072 2a00 0000 7214  ....r(...r*...r.
+000012d0: 0000 0072 1500 0000 7218 0000 0072 1900  ...r....r....r..
+000012e0: 0000 7219 0000 0072 1a00 0000 da1f 7072  ..r....r......pr
+000012f0: 6563 6f6d 7075 7465 5f6d 6f64 6974 5f64  ecompute_modit_d
+00001300: 6974 6772 6964 5f6d 6174 7269 7879 0000  itgrid_matrixy..
+00001310: 0073 2000 0000 000b 0a01 2001 2001 0e01  .s ....... . ...
+00001320: 0401 1201 0801 0e01 0801 0801 0801 1c02  ................
+00001330: 0e01 0c01 0a01 722f 0000 0029 0272 0200  ......r/...).r..
+00001340: 0000 5429 0372 0200 0000 4e54 2902 7202  ..T).r....NT).r.
+00001350: 0000 0054 2902 7202 0000 0054 2902 7202  ...T).r....T).r.
+00001360: 0000 0054 2909 da07 5f5f 646f 635f 5fda  ...T)...__doc__.
+00001370: 056e 756d 7079 7207 0000 00da 0877 6172  .numpyr......war
+00001380: 6e69 6e67 7372 1b00 0000 721d 0000 0072  ningsr....r....r
+00001390: 2b00 0000 722d 0000 0072 2f00 0000 7219  +...r-...r/...r.
+000013a0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000013b0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000013c0: 730e 0000 0004 0608 0108 020a 190a 1d0a  s...............
+000013d0: 200a 19                                   ..
```

## exojax/spec/__pycache__/unitconvert.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:28:50 2023 UTC, .py size: 727 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 d28f 1164 d702 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 d702 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 5a00 6407 6402 6403 8401 5a01 6404 6405  Z.d.d.d...Z.d.d.
 00000040: 8400 5a02 6406 5300 2908 7a1d 756e 6974  ..Z.d.S.).z.unit
 00000050: 2063 6f6e 7665 7273 696f 6e20 666f 7220   conversion for 
 00000060: 7370 6563 7472 756d 2eda 0241 4163 0200  spectrum...AAc..
 00000070: 0000 0000 0000 0000 0000 0200 0000 0500  ................
```

## exojax/test/__pycache__/__init__.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Dec  7 12:18:00 2022 UTC, .py size: 14 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7884 9063 0e00 0000  U.......x..c....
+00000000: 550d 0d0a 0000 0000 750a 3264 0e00 0000  U.......u.2d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0800 0000 6700  .....@...s....g.
 00000030: 5a00 6400 5300 2901 4e29 01da 075f 5f61  Z.d.S.).N)...__a
 00000040: 6c6c 5f5f a900 7202 0000 0072 0200 0000  ll__..r....r....
 00000050: fa34 6275 696c 642f 6264 6973 742e 6c69  .4build/bdist.li
 00000060: 6e75 782d 7838 365f 3634 2f65 6767 2f65  nux-x86_64/egg/e
 00000070: 786f 6a61 782f 7465 7374 2f5f 5f69 6e69  xojax/test/__ini
```

## exojax/test/__pycache__/data.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 1666 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 8206 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 8206 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6409 5a09 640a 5a0a 640b 5a0b 640c  Z.d.Z.d.Z.d.Z.d.
 00000060: 5a0c 640d 5a0d 640e 5a0e 640f 5a0f 6410  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a10 6411 5a11 6412 5a12 6413 5a13 6414  Z.d.Z.d.Z.d.Z.d.
```

## exojax/test/__pycache__/emulate_broadpar.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Feb  6 13:31:25 2023 UTC, .py size: 807 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2d01 e163 2703 0000  U.......-..c'...
+00000000: 550d 0d0a 0000 0000 f75d 7864 2703 0000  U........]xd'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6403 6404 8400  Z.d.d.l.Z.d.d...
 00000040: 5a03 6405 6406 8400 5a04 6402 5300 2907  Z.d.d...Z.d.S.).
 00000050: 7a4c 656d 756c 6174 6520 6272 6f61 6465  zLemulate broade
 00000060: 6e69 6e67 2070 6172 616d 6574 6572 7320  ning parameters 
 00000070: 666f 7220 756e 6974 2074 6573 742c 2075  for unit test, u
```

## exojax/test/__pycache__/emulate_mdb.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 2774 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 d60a 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 d60a 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6406 6407 8400 5a0b 6408  m.Z...d.d...Z.d.
```

## exojax/test/__pycache__/generate.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 1843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 3307 0000  U.......!..d3...
+00000000: 550d 0d0a 0000 0000 c50a 3264 3307 0000  U.........2d3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 6401 6404 6c06 5a06 6401 6405 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6508 a009 6406 6407 a102  m.Z...e...d.d...
 00000070: 0100 6408 6409 8400 5a0a 640a 640b 8400  ..d.d...Z.d.d...
```

## exojax/test/__pycache__/generate_mdb.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 2591 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 1f0a 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 d70a 3264 1f0a 0000  U.........2d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 6405 6406 8400 5a06 6407 6408 8400  Z.d.d...Z.d.d...
 00000060: 5a07 6508 6409 6b02 7262 6506 640a 8301  Z.e.d.k.rbe.d...
 00000070: 0100 6506 640b 8301 0100 6506 640c 8301  ..e.d.....e.d...
```

## exojax/test/__pycache__/generate_methane_spectrum.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 ce0c 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 f75d 7864 ce0c 0000  U........]xd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 2002 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a05 0100 6401 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6404 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6401 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

## exojax/test/__pycache__/generate_rt.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 4139 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 2b10 0000  U.......!..d+...
+00000000: 550d 0d0a 0000 0000 f75d 7864 2b10 0000  U........]xd+...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0a02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c06 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6401 6c0a 6d0b 5a0c 0100 6400  ..d.d.l.m.Z...d.
```

## exojax/test/__pycache__/generate_xs.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 4954 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 5a13 0000  U.......!..dZ...
+00000000: 550d 0d0a 0000 0000 f75d 7864 5a13 0000  U........]xdZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2802 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 5a05 6400 6405 6c06  ..d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6400 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
```

## exojax/utils/__pycache__/constants.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 1574 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 2606 0000  U.......!..d&...
+00000000: 550d 0d0a 0000 0000 f75d 7864 2606 0000  U........]xd&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6409 5a09 640a 5a0a 640b 5a0b 640c  Z.d.Z.d.Z.d.Z.d.
 00000060: 5a0c 640d 5a0d 640e 5a0e 640f 5a0f 6410  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a10 6411 5a11 6412 5a12 6413 5a13 6414  Z.d.Z.d.Z.d.Z.d.
```

## exojax/utils/__pycache__/grids.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 5441 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 4115 0000  U.......!..dA...
+00000000: 550d 0d0a 0000 0000 f75d 7864 4115 0000  U........]xdA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0b 0100 6401 6405 6c0a  d.l.m.Z...d.d.l.
 00000070: 5a0c 6401 6405 6c0d 5a0d 6421 6407 6408  Z.d.d.l.Z.d!d.d.
```

## exojax/utils/__pycache__/instfunc.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 1554 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 1206 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 e566 1664 1206 0000  U........f.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6402 6c05 5a05 6404  m.Z...d.d.l.Z.d.
 00000050: 6405 8400 5a06 6406 6407 8400 5a07 6408  d...Z.d.d...Z.d.
 00000060: 6409 8400 5a08 640a 640b 8400 5a09 640c  d...Z.d.d...Z.d.
 00000070: 640d 8400 5a0a 6402 5300 290e 7a25 5574  d...Z.d.S.).z%Ut
```

## exojax/utils/__pycache__/molname.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 09:34:25 2023 UTC, .py size: 6145 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2191 1164 0118 0000  U.......!..d....
+00000000: 550d 0d0a 0000 0000 e566 1664 0118 0000  U........f.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6403 6404 8400  Z.d.d.l.Z.d.d...
 00000050: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
 00000060: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
 00000070: 5a08 640d 640e 8400 5a09 640f 6410 8400  Z.d.d...Z.d.d...
```

