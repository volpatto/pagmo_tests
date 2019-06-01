cmake_minimum_required(VERSION 3.14)

project(pagmo_tests)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")

include_directories(examples)
include_directories(
        $ENV{HOME}/miniconda3/envs/pagmo_env/include
        $ENV{HOME}/miniconda3/envs/pagmo_env/include/eigen3
)

add_executable(pagmo_tests examples/quickstart.cpp)
