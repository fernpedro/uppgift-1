cmake_minimum_required(VERSION 3.10)
project(MyProject VERSION 1.0.0)

add_library(say-hello hello.hpp hello.cpp)

add_executable(cmake-1a main.cpp)
#add_executable(cmake-1a main.cpp hello.cpp)
target_link_libraries(cmake-1a PRIVATE say-hello)