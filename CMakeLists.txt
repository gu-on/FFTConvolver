cmake_minimum_required(VERSION 3.20)

project(fftconvolver VERSION 1.0 LANGUAGES CXX)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")

option(BUILD_TEST "Whether or not to build tests" OFF)

if(BUILD_TEST)
    enable_testing()
    add_subdirectory(test)
endif()

add_subdirectory(src)

target_compile_features(fftconvolver
    PRIVATE cxx_std_11
)