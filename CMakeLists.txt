cmake_minimum_required(VERSION 3.20)

project(fftconvolver VERSION 1.0 LANGUAGES CXX)

enable_testing()

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")

add_subdirectory(src)
add_subdirectory(test)