cmake_minimum_required(VERSION 2.18) 

project("Hello" CXX)

add_library(libCalc STATIC calculator.cpp)

add_executable("${PROJECT_NAME}" main.cpp)

target_link_libraries("${PROJECT_NAME}" libCalc)
