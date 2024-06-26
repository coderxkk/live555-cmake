#cmake_minimum_required(VERSION 3.27)
#project(BasicUsageEnvironment)

file(GLOB_RECURSE groupsock_src *.cpp )
file(GLOB_RECURSE groupsock_c_src *.c )


add_library(groupsock ${groupsock_src} ${groupsock_c_src})