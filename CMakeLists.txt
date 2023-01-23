cmake_minimum_required(VERSION 3.23)

project(xtest)

set(CMAKE_CXX_STANDARD 17)

add_executable(xtest main.cpp)

find_library(XERCES_LIB xerces-c)

target_link_libraries(xtest PRIVATE "${XERCES_LIB}")
