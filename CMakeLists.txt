cmake_minimum_required(VERSION 2.8)

include(Doxygen/doxygen.cmake)

if( CMAKE_CXX_COMPILER_ID MATCHES "Clang" )
    set(CMAKE_CXX_FLAGS "-Weverything -std=c++14 -Wno-c++98-compat -Wno-c++98-compat-pedantic -Wno-c++98-c++11-compat -Wno-c++98-c++11-compat-pedantic")
    set(CMAKE_C_FLAGS "-Weverything")
else()
    set(CMAKE_CXX_FLAGS "-Wall -Wextra -std=c++14")
    set(CMAKE_C_FLAGS "-Wall -Wextra")
endif()

include_directories(include)

add_subdirectory(Main)
add_subdirectory(Sub)

