cmake_minimum_required(VERSION 2.8)

set(source_files 
    ${CMAKE_CURRENT_SOURCE_DIR}/main.cpp)
add_executable(Main ${source_files})
add_doxygen(Main)

target_link_libraries(Main Sub)
