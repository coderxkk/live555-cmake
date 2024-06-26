file(GLOB test_list test*.cpp)
set (test_list2 "")
list(APPEND test_list2  mikeyPath.cpp)
list(APPEND test_list2  MPEG2TransportStreamIndexer.cpp)
list(APPEND test_list2  playCommon.cpp)
list(APPEND test_list2  registerRTSPStream.cpp)
list(APPEND test_list2  sapWatch.cpp)
list(APPEND test_list2  vobStreamer.cpp)


foreach (file ${test_list})

    get_filename_component(file_name ${file} NAME_WE)

    add_executable(${file_name} ${file} announceURL.cpp)
    target_link_libraries(${file_name} liveMedia BasicUsageEnvironment UsageEnvironment groupsock  ws2_32)
endforeach ()

