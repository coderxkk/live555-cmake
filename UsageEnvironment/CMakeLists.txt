#cmake_minimum_required(VERSION 3.27)
#project(UsageEnvironment)

file(GLOB_RECURSE usage_environment_src *.cpp )
#message(STATUS "UsageEnvironment source file")

#foreach (usage_src ${usage_environment_src})
#    message(STATUS ${usage_src})
#endforeach ()

add_library(UsageEnvironment ${usage_environment_src})
