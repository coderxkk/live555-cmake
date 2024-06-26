#cmake_minimum_required(VERSION 3.27)
#project(BasicUsageEnvironment)

file(GLOB_RECURSE live_media_src *.cpp )
file(GLOB_RECURSE live_media_c_src *.c )
#message(STATUS "liveMedia source file")

add_library(liveMedia ${live_media_src} ${live_media_c_src})