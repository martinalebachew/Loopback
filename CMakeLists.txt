# CMakeLists.txt
# (C) Martin Alebachew, 2024

cmake_minimum_required(VERSION 3.8)
project(loopback-demo C CXX)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/../bin)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY_DEBUG ${CMAKE_BINARY_DIR}/../bin)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY_RELEASE ${CMAKE_BINARY_DIR}/../bin)

file(GLOB SOURCES src/*.cpp src/*/*.cpp src/*/*/*.cpp)
add_executable(loopback ${SOURCES})
