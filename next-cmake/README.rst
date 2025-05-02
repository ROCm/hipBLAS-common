.. highlight:: rst
.. |project_name| replace:: hipBLAS-common

==============
|project_name|
==============

-----------------
Quick Start Guide
-----------------

|project_name| is a header-only library that provides common files for hipBLAS and hipBLASLt.

This section describes how to configure and build the |project_name| project. We assume the user has a
ROCm installation, Python 3.8 or newer and CMake 3.25.0 or newer.

^^^^^^^^^^^^^^^^^^^
Configure and Build
^^^^^^^^^^^^^^^^^^^

|project_name| provides modern CMake support and relies on native CMake functionality with exception of
some project specific options. As such, users are advised to refer to the CMake documentation for
general usage questions. Below are usage examples to get started. For details on all configuration
options see the options section.

Build and Install |project_name|
--------------------------------

   .. code-block:: bash
      :linenos:

      cd hipBLAS-common
      # configure
      CC=/opt/rocm/bin/amdclang++              \
      CXX=/opt/rocm/bin/amdclang++             \
      cmake -B build                           \
            -S next-cmake                      \
            -D CMAKE_INSTALL_PREFIX=$ROCM_PATH
      # build and install
      cmake --build build
      cmake --install build

Options
-------

|project_name| is a header-only library and does not have any custom build options.

CMake Targets
-------------

* ``hip::hipblas-common``
* ``roc::hipblas-common`` (deprecated)
