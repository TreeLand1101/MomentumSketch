cmake_minimum_required(VERSION 3.14)
project(ParameterHeatmap)

set(CMAKE_CXX_STANDARD 17)

add_compile_options(-O1 -mavx2 -mfma -mbmi2 -march=native)

include_directories(../../Common)
include_directories(../../Struct)
include_directories(../../Src)

add_executable(TwoStageParameter TwoStageParameter.cpp  ../../Common/murmur3.c)