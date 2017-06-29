cmake_minimum_required(VERSION 3.6)
project(lab03-master)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp temp.cc)

add_executable(test_input test_input.cc temp.cc)

add_executable(lab03-master ${SOURCE_FILES})

enable_testing()
add_test(NAME test_input COMMAND test_input)
