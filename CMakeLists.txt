cmake_minimum_required(VERSION 3.24)
project(cudadistance CUDA)

set(CMAKE_CUDA_STANDARD 11)

add_library(cudadistance library.cu)

set_target_properties(cudadistance PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
