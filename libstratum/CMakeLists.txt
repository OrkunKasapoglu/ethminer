set(SOURCES
    EthStratumClient.h EthStratumClient.cpp
)

add_library(ethstratum ${SOURCES})
target_link_libraries(ethstratum PUBLIC devcore Boost::system jsoncpp_lib_static)
target_include_directories(ethstratum PRIVATE ..)
