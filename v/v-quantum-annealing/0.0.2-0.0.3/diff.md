# Comparing `tmp/v_quantum_annealing-0.0.2.tar.gz` & `tmp/v_quantum_annealing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v_quantum_annealing-0.0.2.tar", last modified: Mon May 29 05:00:41 2023, max compression
+gzip compressed data, was "v_quantum_annealing-0.0.3.tar", last modified: Thu Jun  1 15:17:17 2023, max compression
```

## Comparing `v_quantum_annealing-0.0.2.tar` & `v_quantum_annealing-0.0.3.tar`

### file list

```diff
@@ -1,187 +1,188 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.540875 v_quantum_annealing-0.0.2/
--rw-rw-rw-   0        0        0     8738 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.2/CMakeLists.txt
--rw-rw-rw-   0        0        0       72 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11560 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1289 2023-05-27 18:46:55.000000 v_quantum_annealing-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1285 2023-05-29 05:00:41.540875 v_quantum_annealing-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9327 2023-05-29 04:48:46.000000 v_quantum_annealing-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.156904 v_quantum_annealing-0.0.2/cmake/
--rw-rw-rw-   0        0        0     5390 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/cmake/FindGcov.cmake
--rw-rw-rw-   0        0        0    13074 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/cmake/FindLcov.cmake
--rw-rw-rw-   0        0        0     9299 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/cmake/Findcodecov.cmake
--rw-rw-rw-   0        0        0     4712 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/cmake/GenerateDocs.cmake
--rw-rw-rw-   0        0        0     2000 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/cmake/PythonAutoDetectOSX.cmake
--rw-rw-rw-   0        0        0     1129 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/cmake/llvm-cov-wrapper
--rw-rw-rw-   0        0        0     1257 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/doc-requirements.in
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.165879 v_quantum_annealing-0.0.2/external/
--rw-rw-rw-   0        0        0     1037 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/external/cimod.cmake
--rw-rw-rw-   0        0        0     1704 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/external/eigen.cmake
--rw-rw-rw-   0        0        0      724 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/external/googletest.cmake
--rw-rw-rw-   0        0        0      781 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/external/json.cmake
--rw-rw-rw-   0        0        0      465 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/external/pybind11-json.cmake
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.166876 v_quantum_annealing-0.0.2/include/
--rw-rw-rw-   0        0        0     2163 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.2/include/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.021265 v_quantum_annealing-0.0.2/include/v_quantum_annealing/
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.169868 v_quantum_annealing-0.0.2/include/v_quantum_annealing/algorithm/
--rw-rw-rw-   0        0        0     3244 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/algorithm/algorithm.hpp
--rw-rw-rw-   0        0        0      731 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/algorithm/all.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.201783 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/
--rw-rw-rw-   0        0        0     1154 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/all.hpp
--rw-rw-rw-   0        0        0     9658 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0    15482 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/chimera.hpp
--rw-rw-rw-   0        0        0      899 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/converter.hpp
--rw-rw-rw-   0        0        0     5269 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/csr_sparse.hpp
--rw-rw-rw-   0        0        0     7702 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/dense.hpp
--rw-rw-rw-   0        0        0     2615 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/graph.hpp
--rw-rw-rw-   0        0        0     9603 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.203778 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/json/
--rw-rw-rw-   0        0        0     4480 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/json/parse.hpp
--rw-rw-rw-   0        0        0    11232 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     8327 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/sparse.hpp
--rw-rw-rw-   0        0        0    10622 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/square.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.212755 v_quantum_annealing-0.0.2/include/v_quantum_annealing/result/
--rw-rw-rw-   0        0        0      731 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/result/all.hpp
--rw-rw-rw-   0        0        0     5217 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/result/get_solution.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.216743 v_quantum_annealing-0.0.2/include/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0    10635 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/sampler/sa_sampler.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.334427 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/
--rw-rw-rw-   0        0        0     1152 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/CMakeLists.txt
--rw-rw-rw-   0        0        0     1410 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/all.hpp
--rw-rw-rw-   0        0        0     6308 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     7212 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/classical_ising.hpp
--rw-rw-rw-   0        0        0    21835 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0    15181 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/continuous_time_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.340412 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.347397 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/
--rw-rw-rw-   0        0        0     5615 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
--rw-rw-rw-   0        0        0    14615 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
--rw-rw-rw-   0        0        0     1750 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
--rw-rw-rw-   0        0        0     2898 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
--rw-rw-rw-   0        0        0    16618 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
--rw-rw-rw-   0        0        0     5502 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0    24738 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/k_local_polynomial.hpp
--rw-rw-rw-   0        0        0      856 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/sa_system.hpp
--rw-rw-rw-   0        0        0     3417 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/system.hpp
--rw-rw-rw-   0        0        0    19954 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/transverse_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.362354 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/
--rw-rw-rw-   0        0        0     1089 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/all.hpp
--rw-rw-rw-   0        0        0    19616 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
--rw-rw-rw-   0        0        0     5468 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/gpu.hpp
--rw-rw-rw-   0        0        0     3889 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/k_local.hpp
--rw-rw-rw-   0        0        0    13765 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/single_spin_flip.hpp
--rw-rw-rw-   0        0        0     6522 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.384295 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/
--rw-rw-rw-   0        0        0     1055 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/create_geometric_progression.hpp
--rw-rw-rw-   0        0        0     1179 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
--rw-rw-rw-   0        0        0     5958 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/eigen.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.385293 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/fmath/
--rw-rw-rw-   0        0        0    26304 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/fmath/fmath.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.390279 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/
--rw-rw-rw-   0        0        0     8427 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/cublas.hpp
--rw-rw-rw-   0        0        0     3061 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/handle_error.hpp
--rw-rw-rw-   0        0        0     2701 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/memory.hpp
--rw-rw-rw-   0        0        0     1102 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/index_type.hpp
--rw-rw-rw-   0        0        0     1337 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/insert_or_assign.hpp
--rw-rw-rw-   0        0        0     1118 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/memory.hpp
--rw-rw-rw-   0        0        0     3673 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/pairhash.hpp
--rw-rw-rw-   0        0        0     4054 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/random.hpp
--rw-rw-rw-   0        0        0    10636 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/schedule_list.hpp
--rw-rw-rw-   0        0        0      853 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/thres_hold.hpp
--rw-rw-rw-   0        0        0     2444 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/type_traits.hpp
--rw-rw-rw-   0        0        0     2309 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/union_find.hpp
--rw-rw-rw-   0        0        0     4681 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1578 2023-05-29 05:00:41.546861 v_quantum_annealing-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-05-29 05:00:25.000000 v_quantum_annealing-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.412221 v_quantum_annealing-0.0.2/tests/
--rw-rw-rw-   0        0        0     1756 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.2/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0        0 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.428185 v_quantum_annealing-0.0.2/tests/__pycache__/
--rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.2/tests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    13004 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_gpu.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    34580 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     5551 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     8200 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     1848 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     2147 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.2/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.433164 v_quantum_annealing-0.0.2/tests/cxxtest/
--rw-rw-rw-   0        0        0     1979 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/cxxtest.cpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.440146 v_quantum_annealing-0.0.2/tests/cxxtest/graph/
--rw-rw-rw-   0        0        0      809 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/graph/all.hpp
--rw-rw-rw-   0        0        0     6134 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0     5917 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/graph/ising_polynomial_model.hpp
--rw-rw-rw-   0        0        0     4604 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     7083 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/graph/quadratic.hpp
--rw-rw-rw-   0        0        0    39029 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/polynomial_test.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.444135 v_quantum_annealing-0.0.2/tests/cxxtest/result/
--rw-rw-rw-   0        0        0      700 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/result/all.hpp
--rw-rw-rw-   0        0        0     2777 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/result/result.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.460092 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/
--rw-rw-rw-   0        0        0      891 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/all.hpp
--rw-rw-rw-   0        0        0     2441 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     3200 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/gpu.hpp
--rw-rw-rw-   0        0        0     2429 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     4313 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/k_local.hpp
--rw-rw-rw-   0        0        0     5337 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/polynomial.hpp
--rw-rw-rw-   0        0        0     6406 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/quadraitc.hpp
--rw-rw-rw-   0        0        0     6808 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/sampler/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.475054 v_quantum_annealing-0.0.2/tests/cxxtest/system/
--rw-rw-rw-   0        0        0      861 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/system/all.hpp
--rw-rw-rw-   0        0        0     7840 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     1390 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/system/classical_ising.hpp
--rw-rw-rw-   0        0        0     4090 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0     9332 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     2447 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/system/k_local.hpp
--rw-rw-rw-   0        0        0    15804 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/testcase.hpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.492006 v_quantum_annealing-0.0.2/tests/cxxtest/utility/
--rw-rw-rw-   0        0        0      744 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/utility/all.hpp
--rw-rw-rw-   0        0        0     3829 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/utility/eigen.hpp
--rw-rw-rw-   0        0        0     6403 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/utility/gpu.hpp
--rw-rw-rw-   0        0        0     1965 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/tests/cxxtest/utility/union_find.hpp
--rw-rw-rw-   0        0        0    28004 2023-05-29 03:26:14.000000 v_quantum_annealing-0.0.2/tests/test_cxx.py
--rw-rw-rw-   0        0        0     5754 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/tests/test_gpu.py
--rw-rw-rw-   0        0        0    60920 2023-05-29 03:36:19.000000 v_quantum_annealing-0.0.2/tests/test_hubo.py
--rw-rw-rw-   0        0        0     6313 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/tests/test_model.py
--rw-rw-rw-   0        0        0    10119 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/tests/test_sampler.py
--rw-rw-rw-   0        0        0     1181 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/tests/test_sqa.py
--rw-rw-rw-   0        0        0     1973 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.505971 v_quantum_annealing-0.0.2/v_quantum_annealing/
--rw-rw-rw-   0        0        0     2240 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/CMakeLists.txt
--rw-rw-rw-   0        0        0     1071 2023-05-29 03:40:46.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/__init__.py
--rw-rw-rw-   0        0        0     2988 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/compile_config.hpp
--rw-rw-rw-   0        0        0    44951 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/declare.hpp
--rw-rw-rw-   0        0        0    15576 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/main.cpp
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.091079 v_quantum_annealing-0.0.2/v_quantum_annealing/model/
--rw-rw-rw-   0        0        0      887 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/model/__init__.py
--rw-rw-rw-   0        0        0    14286 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/model/chimera_model.py
--rw-rw-rw-   0        0        0     9035 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/model/king_graph.py
--rw-rw-rw-   0        0        0    23582 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/model/model.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.107036 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0      529 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/__init__.py
--rw-rw-rw-   0        0        0     4272 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/base_sa_sample_hubo.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.114017 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/
--rw-rw-rw-   0        0        0      320 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
--rw-rw-rw-   0        0        0     5010 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-rw-rw-   0        0        0     5847 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-rw-rw-   0        0        0     5240 2023-05-28 14:52:35.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/csqa_sampler.py
--rw-rw-rw-   0        0        0     1124 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/response.py
--rw-rw-rw-   0        0        0    25532 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/sa_sampler.py
--rw-rw-rw-   0        0        0     8979 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/sampler.py
--rw-rw-rw-   0        0        0    12920 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/sqa_sampler.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.146929 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/
--rw-rw-rw-   0        0        0      767 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/__init__.py
--rw-rw-rw-   0        0        0    10152 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/benchmark.py
--rw-rw-rw-   0        0        0     1283 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/cxx_cast.py
--rw-rw-rw-   0        0        0      855 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/decorator.py
--rw-rw-rw-   0        0        0      992 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/graph_utils.py
--rw-rw-rw-   0        0        0     2120 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/res_convertor.py
--rw-rw-rw-   0        0        0       36 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/utils/time_measure.py
--rw-rw-rw-   0        0        0     1010 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.2/v_quantum_annealing/variable_type.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:00:41.533895 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/
--rw-rw-rw-   0        0        0     1285 2023-05-29 05:00:40.000000 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7487 2023-05-29 05:00:40.000000 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 05:00:40.000000 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 08:08:59.000000 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-05-29 05:00:40.000000 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-29 05:00:40.000000 v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.701212 v_quantum_annealing-0.0.3/
+-rw-rw-rw-   0        0        0     8922 2023-06-01 15:12:03.000000 v_quantum_annealing-0.0.3/CMakeLists.txt
+-rw-rw-rw-   0        0        0       72 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11560 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1289 2023-05-27 18:46:55.000000 v_quantum_annealing-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1285 2023-06-01 15:17:17.701212 v_quantum_annealing-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9339 2023-06-01 09:51:29.000000 v_quantum_annealing-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.400538 v_quantum_annealing-0.0.3/cmake/
+-rw-rw-rw-   0        0        0     5390 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/cmake/FindGcov.cmake
+-rw-rw-rw-   0        0        0    13074 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/cmake/FindLcov.cmake
+-rw-rw-rw-   0        0        0     9299 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/cmake/Findcodecov.cmake
+-rw-rw-rw-   0        0        0     4712 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/cmake/GenerateDocs.cmake
+-rw-rw-rw-   0        0        0     2000 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/cmake/PythonAutoDetectOSX.cmake
+-rw-rw-rw-   0        0        0     1129 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/cmake/llvm-cov-wrapper
+-rw-rw-rw-   0        0        0     1257 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/doc-requirements.in
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.407520 v_quantum_annealing-0.0.3/external/
+-rw-rw-rw-   0        0        0     1037 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/external/cimod.cmake
+-rw-rw-rw-   0        0        0     1704 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/external/eigen.cmake
+-rw-rw-rw-   0        0        0      724 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/external/googletest.cmake
+-rw-rw-rw-   0        0        0      781 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/external/json.cmake
+-rw-rw-rw-   0        0        0      465 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/external/pybind11-json.cmake
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.410510 v_quantum_annealing-0.0.3/include/
+-rw-rw-rw-   0        0        0     2199 2023-06-01 14:56:58.000000 v_quantum_annealing-0.0.3/include/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.283338 v_quantum_annealing-0.0.3/include/v_quantum_annealing/
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.415497 v_quantum_annealing-0.0.3/include/v_quantum_annealing/algorithm/
+-rw-rw-rw-   0        0        0     3244 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/algorithm/algorithm.hpp
+-rw-rw-rw-   0        0        0      731 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/algorithm/all.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.438436 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/
+-rw-rw-rw-   0        0        0     1154 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/all.hpp
+-rw-rw-rw-   0        0        0     9658 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    15482 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/chimera.hpp
+-rw-rw-rw-   0        0        0      899 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/converter.hpp
+-rw-rw-rw-   0        0        0     5269 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/csr_sparse.hpp
+-rw-rw-rw-   0        0        0     7702 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/dense.hpp
+-rw-rw-rw-   0        0        0     2615 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/graph.hpp
+-rw-rw-rw-   0        0        0     9603 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.439432 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/json/
+-rw-rw-rw-   0        0        0     4480 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/json/parse.hpp
+-rw-rw-rw-   0        0        0    11232 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     8327 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/sparse.hpp
+-rw-rw-rw-   0        0        0    10622 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/square.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.446414 v_quantum_annealing-0.0.3/include/v_quantum_annealing/result/
+-rw-rw-rw-   0        0        0      731 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/result/all.hpp
+-rw-rw-rw-   0        0        0     5217 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/result/get_solution.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.448408 v_quantum_annealing-0.0.3/include/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0    10635 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/sampler/sa_sampler.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.470350 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/
+-rw-rw-rw-   0        0        0     1152 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1410 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/all.hpp
+-rw-rw-rw-   0        0        0     6308 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     7212 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0    21835 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0    15181 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/continuous_time_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.474339 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.485310 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/
+-rw-rw-rw-   0        0        0     5615 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
+-rw-rw-rw-   0        0        0    14615 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
+-rw-rw-rw-   0        0        0     1750 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
+-rw-rw-rw-   0        0        0     2898 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
+-rw-rw-rw-   0        0        0    16618 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
+-rw-rw-rw-   0        0        0     5502 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0    24738 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/k_local_polynomial.hpp
+-rw-rw-rw-   0        0        0      856 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/sa_system.hpp
+-rw-rw-rw-   0        0        0     3417 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/system.hpp
+-rw-rw-rw-   0        0        0    19954 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/transverse_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.499272 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/
+-rw-rw-rw-   0        0        0     1089 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/all.hpp
+-rw-rw-rw-   0        0        0    19616 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
+-rw-rw-rw-   0        0        0     5468 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/gpu.hpp
+-rw-rw-rw-   0        0        0     3889 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/k_local.hpp
+-rw-rw-rw-   0        0        0    13765 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/single_spin_flip.hpp
+-rw-rw-rw-   0        0        0     6522 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.522211 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/
+-rw-rw-rw-   0        0        0     1055 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/create_geometric_progression.hpp
+-rw-rw-rw-   0        0        0     1179 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     5958 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/eigen.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.524206 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/fmath/
+-rw-rw-rw-   0        0        0    26304 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/fmath/fmath.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.533182 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/
+-rw-rw-rw-   0        0        0     8427 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/cublas.hpp
+-rw-rw-rw-   0        0        0     3061 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/handle_error.hpp
+-rw-rw-rw-   0        0        0     2701 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/memory.hpp
+-rw-rw-rw-   0        0        0     1102 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/index_type.hpp
+-rw-rw-rw-   0        0        0     1337 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/insert_or_assign.hpp
+-rw-rw-rw-   0        0        0     1118 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/memory.hpp
+-rw-rw-rw-   0        0        0     3673 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/pairhash.hpp
+-rw-rw-rw-   0        0        0     4054 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/random.hpp
+-rw-rw-rw-   0        0        0    10636 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/schedule_list.hpp
+-rw-rw-rw-   0        0        0      853 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/thres_hold.hpp
+-rw-rw-rw-   0        0        0     2444 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/type_traits.hpp
+-rw-rw-rw-   0        0        0     2309 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/union_find.hpp
+-rw-rw-rw-   0        0        0     4681 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1578 2023-06-01 15:17:17.703208 v_quantum_annealing-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-01 15:17:13.000000 v_quantum_annealing-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.560623 v_quantum_annealing-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1756 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.3/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.583561 v_quantum_annealing-0.0.3/tests/__pycache__/
+-rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.3/tests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13004 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_gpu.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    34580 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     5551 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     8200 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     1848 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     2147 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.3/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.590542 v_quantum_annealing-0.0.3/tests/cxxtest/
+-rw-rw-rw-   0        0        0     1979 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/cxxtest.cpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.603509 v_quantum_annealing-0.0.3/tests/cxxtest/graph/
+-rw-rw-rw-   0        0        0      809 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/graph/all.hpp
+-rw-rw-rw-   0        0        0     6134 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     5917 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/graph/ising_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     4604 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     7083 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/graph/quadratic.hpp
+-rw-rw-rw-   0        0        0    39029 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/polynomial_test.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.624451 v_quantum_annealing-0.0.3/tests/cxxtest/result/
+-rw-rw-rw-   0        0        0      700 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/result/all.hpp
+-rw-rw-rw-   0        0        0     2777 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/result/result.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.646393 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/
+-rw-rw-rw-   0        0        0      891 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/all.hpp
+-rw-rw-rw-   0        0        0     2441 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     3200 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/gpu.hpp
+-rw-rw-rw-   0        0        0     2429 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     4313 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/k_local.hpp
+-rw-rw-rw-   0        0        0     5337 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/polynomial.hpp
+-rw-rw-rw-   0        0        0     6406 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/quadraitc.hpp
+-rw-rw-rw-   0        0        0     6808 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/sampler/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.656367 v_quantum_annealing-0.0.3/tests/cxxtest/system/
+-rw-rw-rw-   0        0        0      861 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/system/all.hpp
+-rw-rw-rw-   0        0        0     7840 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     1390 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0     4090 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0     9332 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     2447 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/system/k_local.hpp
+-rw-rw-rw-   0        0        0    15804 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/testcase.hpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.666339 v_quantum_annealing-0.0.3/tests/cxxtest/utility/
+-rw-rw-rw-   0        0        0      744 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/utility/all.hpp
+-rw-rw-rw-   0        0        0     3829 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/utility/eigen.hpp
+-rw-rw-rw-   0        0        0     6403 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/utility/gpu.hpp
+-rw-rw-rw-   0        0        0     1965 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/tests/cxxtest/utility/union_find.hpp
+-rw-rw-rw-   0        0        0    28004 2023-05-29 03:26:14.000000 v_quantum_annealing-0.0.3/tests/test_cxx.py
+-rw-rw-rw-   0        0        0     5754 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/tests/test_gpu.py
+-rw-rw-rw-   0        0        0    60920 2023-05-29 03:36:19.000000 v_quantum_annealing-0.0.3/tests/test_hubo.py
+-rw-rw-rw-   0        0        0     6313 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/tests/test_model.py
+-rw-rw-rw-   0        0        0    10119 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/tests/test_sampler.py
+-rw-rw-rw-   0        0        0     1181 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/tests/test_sqa.py
+-rw-rw-rw-   0        0        0     1973 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.674284 v_quantum_annealing-0.0.3/v_quantum_annealing/
+-rw-rw-rw-   0        0        0     2240 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1126 2023-06-01 10:09:12.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-06-01 10:54:31.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/_version.py
+-rw-rw-rw-   0        0        0     2988 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/compile_config.hpp
+-rw-rw-rw-   0        0        0    44951 2023-05-29 04:48:44.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/declare.hpp
+-rw-rw-rw-   0        0        0    15576 2023-06-01 09:56:41.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/main.cpp
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.353152 v_quantum_annealing-0.0.3/v_quantum_annealing/model/
+-rw-rw-rw-   0        0        0      887 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/model/__init__.py
+-rw-rw-rw-   0        0        0    14286 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/model/chimera_model.py
+-rw-rw-rw-   0        0        0     9035 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/model/king_graph.py
+-rw-rw-rw-   0        0        0    23582 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/model/model.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.368111 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0      529 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/__init__.py
+-rw-rw-rw-   0        0        0     4272 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/base_sa_sample_hubo.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.374095 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/
+-rw-rw-rw-   0        0        0      320 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-rw-rw-   0        0        0     5010 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-rw-rw-   0        0        0     5847 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-rw-rw-   0        0        0     5240 2023-05-28 14:52:35.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/csqa_sampler.py
+-rw-rw-rw-   0        0        0     1124 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/response.py
+-rw-rw-rw-   0        0        0    25532 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/sa_sampler.py
+-rw-rw-rw-   0        0        0     8979 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/sampler.py
+-rw-rw-rw-   0        0        0    12920 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/sqa_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.387580 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/
+-rw-rw-rw-   0        0        0      767 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10152 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/benchmark.py
+-rw-rw-rw-   0        0        0     1283 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/cxx_cast.py
+-rw-rw-rw-   0        0        0      855 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/decorator.py
+-rw-rw-rw-   0        0        0      992 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/graph_utils.py
+-rw-rw-rw-   0        0        0     2120 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/res_convertor.py
+-rw-rw-rw-   0        0        0       36 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/utils/time_measure.py
+-rw-rw-rw-   0        0        0     1010 2023-05-29 04:48:45.000000 v_quantum_annealing-0.0.3/v_quantum_annealing/variable_type.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:17:17.691239 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/
+-rw-rw-rw-   0        0        0     1285 2023-06-01 15:17:16.000000 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7553 2023-06-01 15:17:17.000000 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 15:17:16.000000 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 08:08:59.000000 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-06-01 15:17:16.000000 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-01 15:17:16.000000 v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/top_level.txt
```

### Comparing `v_quantum_annealing-0.0.2/CMakeLists.txt` & `v_quantum_annealing-0.0.3/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,43 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 cmake_minimum_required(VERSION 3.22 FATAL_ERROR)
-project(openjij
+project(v_quantum_annealing
     DESCRIPTION "Framework for the Ising model and QUBO."
-    HOMEPAGE_URL "https://www.openjij.org"
+    HOMEPAGE_URL "https://v-quantum-technology.com/"
 )
 
 # Standard includes
 include(CheckLanguage)
 
-set(OPENJIJ_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)
+set(V_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)
 
 if (CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
     if(CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_CURRENT_BINARY_DIR)
         set(lines "You are building in-place.") 
         message(AUTHOR_WARNING ${lines})
     endif()
-    set(OPENJIJ_MAIN_PROJECT ON)
+    set(V_QUANTUM_ENNEALING_MAIN_PROJECT ON)
     message(STATUS "CMake ${CMAKE_VERSION}")
     if(CMAKE_CXX_STANDARD)
         set(CMAKE_CXX_EXTENSIONS OFF)
         set(CMAKE_CXX_STANDARD_REQUIRED ON)
     endif()
 else()
-  set(OPENJIJ_MAIN_PROJECT OFF)
+  set(V_QUANTUM_ENNEALING_MAIN_PROJECT OFF)
 endif()
 
 # Options
-option(OPENJIJ_INSTALL "Install cimod header files?" ${OPENJIJ_MAIN_PROJECT})
-option(OPENJIJ_TEST "Build cimod test suite?" ${OPENJIJ_MAIN_PROJECT})
-option(OPENJIJ_DOCS "Build cimod docs?" ${OPENJIJ_MAIN_PROJECT})
+option(V_QUANTUM_ENNEALING_INSTALL "Install cimod header files?" ${V_QUANTUM_ENNEALING_MAIN_PROJECT})
+option(V_QUANTUM_ENNEALING_TEST "Build cimod test suite?" ${V_QUANTUM_ENNEALING_MAIN_PROJECT})
+option(V_QUANTUM_ENNEALING_DOCS "Build cimod docs?" ${V_QUANTUM_ENNEALING_MAIN_PROJECT})
 option(BUILD_DOCS "Enable Doxygen support." OFF)
 option(CMAKE_REQUIRE_FAILE "If CMake could not find dependencies, build will faile." OFF)
 
 list(APPEND CMAKE_MODULE_PATH external)
 list(APPEND CMAKE_MODULE_PATH cmake)
 
 check_language(C)
@@ -221,15 +221,15 @@
   message(STATUS "Fetch cimod")
   include(external/cimod.cmake)
 endif()
 
 add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/include)
 
 # Build Python Extension 
-if(SKBUILD AND OPENJIJ_MAIN_PROJECT)
+if(SKBUILD AND V_QUANTUM_ENNEALING_MAIN_PROJECT)
   message(STATUS "Build Python Extension.")
   option(WITH_THREAD "Compile in rudimentary thread support" ON)
   option(BUILD_TESTING "Enable CTest support." OFF)
   find_package(Python3 COMPONENTS Interpreter Development NumPy)
   # Scikit-Build does not add your site-packages to the search path
   # automatically, so we need to add it _or_ the pybind11 specific directory
   # here.
@@ -250,16 +250,16 @@
   if(TARGET pybind11_json)
     message(STATUS "Skip Download pybind11_json")
   else()
     message(STATUS "Downlod pybind11_json")
     include(external/pybind11-json.cmake)
   endif()
   
-  add_subdirectory(openjij)
-elseif(OPENJIJ_MAIN_PROJECT AND ((${CMAKE_BUILD_TYPE} MATCHES Debug) OR OPENJIJ_TEST))
+  add_subdirectory(v_quantum_annealing)
+elseif(V_QUANTUM_ENNEALING_MAIN_PROJECT AND ((${CMAKE_BUILD_TYPE} MATCHES Debug) OR V_QUANTUM_ENNEALING_TEST))
   include(CTest)
   if(ENABLE_COVERAGE AND (NOT MSVC))
     message(STATUS "Use Codecov")
     find_package(codecov)
   endif()
   
   message(STATUS "Use Googletest") 
@@ -271,10 +271,10 @@
   add_subdirectory(tests)
   
   if(ENABLE_COVERAGE AND (NOT MSVC))
      coverage_evaluate()
   endif()
 endif()
 
-if (OPENJIJ_MAIN_PROJECT AND BUILD_DOCS AND OPENJIJ_DOCS)
+if (V_QUANTUM_ENNEALING_MAIN_PROJECT AND BUILD_DOCS AND V_QUANTUM_ENNEALING_DOCS)
     include(cmake/GenerateDocs.cmake)
 endif ()
```

### Comparing `v_quantum_annealing-0.0.2/LICENSE` & `v_quantum_annealing-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/MANIFEST.in` & `v_quantum_annealing-0.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/PKG-INFO` & `v_quantum_annealing-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v_quantum_annealing
-Version: 0.0.2
+Version: 0.0.3
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
```

### Comparing `v_quantum_annealing-0.0.2/README.md` & `v_quantum_annealing-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 - [v_quantum_annealing Slack](https://join.slack.com/t/v_quantum_annealing/shared_invite/enQtNjQyMjIwMzMwNzA4LTQ5MWRjOWYxYmY1Nzk4YzdiYzlmZjIxYjhhMmMxZjAyMzE3MDc1ZWRkYmI1YjhkNjRlOTM1ODE0NTc5Yzk3ZDA)
 
 ## About us
 
 This product is maintained by Jij Inc.
 
 **Please visit our website for more information!**
-https://www.j-ij.com/
+https://v-quantum-technology.com/
 
 ### Licences
 
 Copyright © 2022-2023 V-QUANTUM Inc. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");\
 you may not use this file except in compliance with the License.\
```

#### html2text {}

```diff
@@ -96,16 +96,16 @@
 sampler.sample_ising(h={0: -1}, J={(0,1): -1}) response.states # [[1,1]] # with
 indices response = sampler.sample_ising(h={'a': -1}, J={('a','b'): 1}) [{index:
 s for index, s in zip(response.indices, state)} for state in response.states] #
 [{'b': -1, 'a': 1}] ``` ## Community - [v_quantum_annealing Slack](https://
 join.slack.com/t/v_quantum_annealing/shared_invite/
 enQtNjQyMjIwMzMwNzA4LTQ5MWRjOWYxYmY1Nzk4YzdiYzlmZjIxYjhhMmMxZjAyMzE3MDc1ZWRkYmI1YjhkNjRlOTM1ODE0NTc5Yzk3ZDA)
 ## About us This product is maintained by Jij Inc. **Please visit our website
-for more information!** https://www.j-ij.com/ ### Licences Copyright Â© 2022-
-2023 V-QUANTUM Inc. All Rights Reserved. Licensed under the Apache License,
-Version 2.0 (the "License");\ you may not use this file except in compliance
-with the License.\ You may obtain a copy of the License at ``` http://
-www.apache.org/licenses/LICENSE-2.0 ``` Unless required by applicable law or
-agreed to in writing, software\ distributed under the License is distributed on
-an "AS IS" BASIS,\ WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
-or implied.\ See the License for the specific language governing permissions
-and\ limitations under the License.
+for more information!** https://v-quantum-technology.com/ ### Licences
+Copyright Â© 2022-2023 V-QUANTUM Inc. All Rights Reserved. Licensed under the
+Apache License, Version 2.0 (the "License");\ you may not use this file except
+in compliance with the License.\ You may obtain a copy of the License at ```
+http://www.apache.org/licenses/LICENSE-2.0 ``` Unless required by applicable
+law or agreed to in writing, software\ distributed under the License is
+distributed on an "AS IS" BASIS,\ WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
+either express or implied.\ See the License for the specific language governing
+permissions and\ limitations under the License.
```

### Comparing `v_quantum_annealing-0.0.2/cmake/FindGcov.cmake` & `v_quantum_annealing-0.0.3/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/cmake/FindLcov.cmake` & `v_quantum_annealing-0.0.3/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/cmake/Findcodecov.cmake` & `v_quantum_annealing-0.0.3/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/cmake/GenerateDocs.cmake` & `v_quantum_annealing-0.0.3/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/cmake/PythonAutoDetectOSX.cmake` & `v_quantum_annealing-0.0.3/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/cmake/llvm-cov-wrapper` & `v_quantum_annealing-0.0.3/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/doc-requirements.in` & `v_quantum_annealing-0.0.3/doc-requirements.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/external/cimod.cmake` & `v_quantum_annealing-0.0.3/external/cimod.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/external/eigen.cmake` & `v_quantum_annealing-0.0.3/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/external/googletest.cmake` & `v_quantum_annealing-0.0.3/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/external/json.cmake` & `v_quantum_annealing-0.0.3/external/json.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/CMakeLists.txt` & `v_quantum_annealing-0.0.3/include/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,47 +8,47 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-message(CHECK_START "cxxjij_header_only")
+message(CHECK_START "cxxvqa_header_only")
 list(APPEND CMAKE_MESSAGE_INDENT "  ")
 
-add_library(cxxjij_header_only INTERFACE)
+add_library(cxxvqa_header_only INTERFACE)
 
 #target_precompile_headers(cxxcimod_header_only INTERFACE
 #    ${CMAKE_CURRENT_SOURCE_DIR}/algorithm/all.hpp
 #    ${CMAKE_CURRENT_SOURCE_DIR}/graph/all.hpp
 #    ${CMAKE_CURRENT_SOURCE_DIR}/result/all.hpp
 #    ${CMAKE_CURRENT_SOURCE_DIR}/system/all.hpp
 #    ${CMAKE_CURRENT_SOURCE_DIR}/updater/all.hpp
 #) 
 
 #for GPU
 if(CUDAToolkit_FOUND)
-    add_subdirectory(openjij/system)
+    add_subdirectory(v_quantum_annealing/system)
 endif()
 
-target_include_directories(cxxjij_header_only INTERFACE 
-  $<BUILD_INTERFACE:${OPENJIJ_INCLUDE_DIR}>
+target_include_directories(cxxvqa_header_only INTERFACE 
+  $<BUILD_INTERFACE:${V-QUANTUM-ANNEALING_INCLUDE_DIR}>
   $<INSTALL_INTERFACE:include>
 )
 
-target_link_libraries(cxxjij_header_only INTERFACE 
+target_link_libraries(cxxvqa_header_only INTERFACE 
     cxxcimod_header_only
     nlohmann_json::nlohmann_json
-    $<IF:$<TARGET_EXISTS:Eigen3::Eigen>,Eigen3::Eigen,openjij-eigen_lib>
+    $<IF:$<TARGET_EXISTS:Eigen3::Eigen>,Eigen3::Eigen,v_quantum_annealing-eigen_lib>
     $<$<TARGET_EXISTS:OpenMP::OpenMP_CXX>:OpenMP::OpenMP_CXX>
     $<$<TARGET_EXISTS:BLAS::BLAS>:BLAS::BLAS>
     $<$<TARGET_EXISTS:LAPACK::LAPACK>:LAPACK::LAPACK>
 )
 
-target_compile_definitions(cxxjij_header_only INTERFACE 
+target_compile_definitions(cxxvqa_header_only INTERFACE 
     EIGEN_MPL2_ONLY
     BUILD_TESTING=OFF
     TEST_LIB=OFF
     EIGEN_BUILD_PKGCONFIG=OFF
     EIGEN_BUILD_DOC=OFF
     EIGEN_DOC_USE_MATHJAX=OFF 
     EIGEN_BUILD_TESTING=OFF
```

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/algorithm/algorithm.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/algorithm/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/algorithm/all.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/algorithm/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/all.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/chimera.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/chimera.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/converter.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/converter.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/csr_sparse.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/csr_sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/dense.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/dense.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/graph.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/graph.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/json/parse.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/json/parse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/polynomial.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/sparse.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/graph/square.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/graph/square.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/result/all.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/result/get_solution.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/result/get_solution.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/sampler/sa_sampler.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/sampler/sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/CMakeLists.txt` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/all.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/classical_ising.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/continuous_time_ising.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/continuous_time_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/k_local_polynomial.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/k_local_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/sa_system.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/system.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/system/transverse_ising.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/system/transverse_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/all.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/gpu.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/k_local.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/single_spin_flip.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/single_spin_flip.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/updater/swendsen_wang.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/updater/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/create_geometric_progression.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/create_geometric_progression.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/disable_eigen_warning.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/eigen.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/fmath/fmath.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/cublas.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/cublas.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/handle_error.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/handle_error.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/gpu/memory.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/gpu/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/index_type.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/index_type.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/insert_or_assign.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/insert_or_assign.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/memory.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/pairhash.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/pairhash.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/random.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/random.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/schedule_list.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/schedule_list.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/thres_hold.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/thres_hold.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/type_traits.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/include/v_quantum_annealing/utility/union_find.hpp` & `v_quantum_annealing-0.0.3/include/v_quantum_annealing/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/pyproject.toml` & `v_quantum_annealing-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/setup.cfg` & `v_quantum_annealing-0.0.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 00000140: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000150: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
 00000160: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
 00000170: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
 00000180: 204c 4943 454e 5345 0d0a 6c69 6365 6e73   LICENSE..licens
 00000190: 6520 3d20 2241 7061 6368 6520 4c69 6365  e = "Apache Lice
 000001a0: 6e73 6520 322e 3022 0d0a 7665 7273 696f  nse 2.0"..versio
-000001b0: 6e20 3d20 2230 2e30 2e32 220d 0a63 6c61  n = "0.0.2"..cla
+000001b0: 6e20 3d20 2230 2e30 2e33 220d 0a63 6c61  n = "0.0.3"..cla
 000001c0: 7373 6966 6965 7273 203d 200d 0a09 4c69  ssifiers = ...Li
 000001d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
 000001e0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
 000001f0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
 00000200: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
 00000210: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
 00000220: 5265 7365 6172 6368 0d0a 0950 726f 6772  Research...Progr
```

### Comparing `v_quantum_annealing-0.0.2/setup.py` & `v_quantum_annealing-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup_requires = [
     "numpy",
     "pybind11 >=2.10.0, < 2.11.0",
     "cmake > 3.20",
     "scikit-build > 0.16.0"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 setup(
     name="v_quantum_annealing", 
     version=__version__,  
     author = "V-QUANTUM JSC",
     author_email = "nqthinh@v-quantum-technology.com",
     setup_requires=setup_requires,
```

### Comparing `v_quantum_annealing-0.0.2/tests/CMakeLists.txt` & `v_quantum_annealing-0.0.3/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.3/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.3/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.3/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.3/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.3/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.3/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/cxxtest.cpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/graph/all.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/graph/polynomial.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/graph/quadratic.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/graph/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/polynomial_test.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/result/all.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/result/result.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/result/result.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/all.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/gpu.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/k_local.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/polynomial.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/quadraitc.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/quadraitc.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/sampler/swendsen_wang.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/sampler/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/system/all.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/system/classical_ising.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/system/k_local.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/system/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/testcase.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/testcase.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/utility/all.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/utility/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/utility/eigen.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/utility/gpu.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/utility/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/cxxtest/utility/union_find.hpp` & `v_quantum_annealing-0.0.3/tests/cxxtest/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_cxx.py` & `v_quantum_annealing-0.0.3/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_gpu.py` & `v_quantum_annealing-0.0.3/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_hubo.py` & `v_quantum_annealing-0.0.3/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_model.py` & `v_quantum_annealing-0.0.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_sampler.py` & `v_quantum_annealing-0.0.3/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_sqa.py` & `v_quantum_annealing-0.0.3/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/tests/test_utils.py` & `v_quantum_annealing-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/CMakeLists.txt` & `v_quantum_annealing-0.0.3/v_quantum_annealing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/__init__.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from pkgutil import extend_path
 __path__ = [] 
 
 __path__ = extend_path(__path__, __name__)
 
+from v_quantum_annealing import cxxvqa
 
 from v_quantum_annealing.model.model import BinaryPolynomialModel, BinaryQuadraticModel
 from v_quantum_annealing.sampler.base_sa_sample_hubo import base_sample_hubo
 from v_quantum_annealing.sampler.csqa_sampler import CSQASampler
 from v_quantum_annealing.sampler.response import Response
 from v_quantum_annealing.sampler.sa_sampler import SASampler
 from v_quantum_annealing.sampler.sqa_sampler import SQASampler
 from v_quantum_annealing.utils.benchmark import solver_benchmark
 from v_quantum_annealing.utils.res_convertor import convert_response
 from v_quantum_annealing.variable_type import BINARY, SPIN, Vartype, cast_vartype
 
 __all__ = [
+    "cxxvqa",
     "SPIN",
     "BINARY",
     "Vartype",
     "cast_vartype",
     "Response",
     "SASampler",
     "SQASampler",
```

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/compile_config.hpp` & `v_quantum_annealing-0.0.3/v_quantum_annealing/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/declare.hpp` & `v_quantum_annealing-0.0.3/v_quantum_annealing/declare.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/main.cpp` & `v_quantum_annealing-0.0.3/v_quantum_annealing/main.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/model/__init__.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/model/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/model/chimera_model.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/model/chimera_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/model/king_graph.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/model/model.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/model/model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/__init__.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/base_sa_sample_hubo.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/base_sa_sample_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/csqa_sampler.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/response.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/response.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/sa_sampler.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/sampler.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/sampler/sqa_sampler.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/utils/__init__.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/utils/benchmark.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/utils/cxx_cast.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/utils/cxx_cast.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/utils/decorator.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/utils/graph_utils.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/utils/res_convertor.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing/variable_type.py` & `v_quantum_annealing-0.0.3/v_quantum_annealing/variable_type.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/PKG-INFO` & `v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v-quantum-annealing
-Version: 0.0.2
+Version: 0.0.3
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
```

### Comparing `v_quantum_annealing-0.0.2/v_quantum_annealing.egg-info/SOURCES.txt` & `v_quantum_annealing-0.0.3/v_quantum_annealing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.md
 doc-requirements.in
 pyproject.toml
 setup.cfg
 setup.py
 ./v_quantum_annealing/__init__.py
+./v_quantum_annealing/_version.py
 ./v_quantum_annealing/variable_type.py
 ./v_quantum_annealing/model/__init__.py
 ./v_quantum_annealing/model/chimera_model.py
 ./v_quantum_annealing/model/king_graph.py
 ./v_quantum_annealing/model/model.py
 ./v_quantum_annealing/sampler/__init__.py
 ./v_quantum_annealing/sampler/base_sa_sample_hubo.py
@@ -141,14 +142,15 @@
 tests/cxxtest/system/k_local.hpp
 tests/cxxtest/utility/all.hpp
 tests/cxxtest/utility/eigen.hpp
 tests/cxxtest/utility/gpu.hpp
 tests/cxxtest/utility/union_find.hpp
 v_quantum_annealing/CMakeLists.txt
 v_quantum_annealing/__init__.py
+v_quantum_annealing/_version.py
 v_quantum_annealing/compile_config.hpp
 v_quantum_annealing/declare.hpp
 v_quantum_annealing/main.cpp
 v_quantum_annealing/variable_type.py
 v_quantum_annealing.egg-info/PKG-INFO
 v_quantum_annealing.egg-info/SOURCES.txt
 v_quantum_annealing.egg-info/dependency_links.txt
```

