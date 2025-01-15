cmake_minimum_required(VERSION 3.15)

project(fftconvolver VERSION 1.0 LANGUAGES CXX)

add_library(fftconvolver STATIC
    src/FFTConvolver.cpp
    src/AudioFFT.cpp
    src/Utilities.cpp
)