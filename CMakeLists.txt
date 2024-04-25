cmake_minimum_required(VERSION 2.8)
project(Factorial)

include_directories(${PROJECT_SOURCE_DIR}/include)
file(GLOB SRC_LIST ${PROJECT_SOURCE_DIR}/src/*.cpp)
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/build/lib)
add_library(factorial STATIC ${SRC_LIST})