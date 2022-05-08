cmake_minimum_required(VERSION 3.22)
project(cfg-checker)

set(CMAKE_CXX_STANDARD 23)

add_executable(cfg-checker main.cpp)

if(NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()

set(CMAKE_CXX_FLAGS "-Wall -Wextra")
set(CMAKE_CXX_FLAGS_DEBUG "-g")
set(CMAKE_CXX_FLAGS_RELEASE "-O3")
