cmake_minimum_required(VERSION 2.8)
project(simulator)
add_subdirectory(src/mimo)
add_subdirectory(src/encoder)
add_executable(simulator src/run.cpp)
target_link_libraries(simulator mimo encoder)
