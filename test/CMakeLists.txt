include(AddCatch2)

add_executable(tests
    Test.cpp
)

target_link_libraries(tests PRIVATE
    Catch2::Catch2WithMain
    fftconvolver
)

include(CTest)
include(Catch)
catch_discover_tests(tests)