cmake_minimum_required(VERSION 3.0.0)
project(cpp VERSION 0.1.0)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(CMAKE_BUILD_TYPE "Debug")

include_directories(csv)
include_directories(const)
include_directories(smart_ptr)

add_executable(smart_ptr smart_ptr/auto_scope.cpp)

add_executable(enum enum/class_enum.cpp)

add_executable(overload overload/overload_inout.cpp)
