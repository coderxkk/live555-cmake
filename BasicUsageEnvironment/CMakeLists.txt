#cmake_minimum_required(VERSION 3.27)
#project(BasicUsageEnvironment)

file(GLOB_RECURSE basic_utils *.cpp )
#message(STATUS "BasicUsageEnvironment source file")
#foreach (basic_src ${basic_utils})
#    message(STATUS ${basic_src})
#endforeach ()
add_library(BasicUsageEnvironment ${basic_utils})