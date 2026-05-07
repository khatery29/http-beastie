cmake_minimum_required(VERSION 3.10)
project(HttpBeastie)

find_package(Boost REQUIRED)

add_executable(HttpServer src/main.cpp src/utils.cpp)

target_include_directories(HttpServer PRIVATE include ${Boost_INCLUDE_DIRS})