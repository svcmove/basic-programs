cmake_minimum_required(VERSION 3.21)

project(Programs LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 23)

add_library(common STATIC program.cpp common.h)

include_directories(.)
add_subdirectory(external/boost)

add_subdirectory(entropy)
add_subdirectory(hexdump)