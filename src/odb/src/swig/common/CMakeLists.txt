# SPDX-License-Identifier: BSD-3-Clause
# Copyright (c) 2019-2025, The OpenROAD Authors

add_library(odb_swig_common
    swig_common.cpp
)

target_include_directories(odb_swig_common
  PUBLIC
    ${PROJECT_SOURCE_DIR}/include
    .
)

target_link_libraries(odb_swig_common
  PUBLIC
    defin
    lefin
    defout
    lefout
    utl_lib
)
