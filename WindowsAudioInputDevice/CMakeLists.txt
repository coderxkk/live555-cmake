file(GLOB device_src *.cpp)
add_executable(show_name ${device_src})
target_link_libraries(show_name liveMedia BasicUsageEnvironment UsageEnvironment groupsock  ws2_32)