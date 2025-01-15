add_library(fftconvolver STATIC
    FFTConvolver.cpp
    TwoStageFFTConvolver.cpp
    AudioFFT.cpp
    Utilities.cpp
)

target_include_directories(fftconvolver PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})