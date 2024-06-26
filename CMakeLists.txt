cmake_minimum_required(VERSION 3.20)
project(live)

set(CMAKE_CXX_STANDARD 14)

add_definitions(-DNO_STD_LIB)
add_definitions(-DNO_GETIFADDRS)
add_definitions(-DNO_OPENSSL)


include_directories(BasicUsageEnvironment/include)
include_directories(groupsock/include)
include_directories(liveMedia)
include_directories(liveMedia/include)
include_directories(mediaServer)
include_directories(testProgs)
include_directories(UsageEnvironment/include)
include_directories(WindowsAudioInputDevice)

add_compile_options(-fPIC)

add_subdirectory(UsageEnvironment)
add_subdirectory(BasicUsageEnvironment)
add_subdirectory(groupsock)
add_subdirectory(liveMedia)
add_subdirectory(hlsProxy)
add_subdirectory(mediaServer)
add_subdirectory(proxyServer)
add_subdirectory(WindowsAudioInputDevice)
add_subdirectory(testProgs)

