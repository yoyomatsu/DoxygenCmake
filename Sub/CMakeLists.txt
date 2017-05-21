cmake_minimum_required(VERSION 2.8)

set(source_files 
    ${CMAKE_CURRENT_SOURCE_DIR}/sub.cpp)
add_library(Sub ${source_files})
add_doxygen(Sub)

