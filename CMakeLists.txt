cmake_minimum_required(VERSION 3.26)
project(tdd)

set(CMAKE_CXX_STANDARD 17)

find_package(Catch2 3 REQUIRED)

add_executable(tests test.cpp
        test.cpp)
target_link_libraries(tests PRIVATE Catch2::Catch2WithMain)
