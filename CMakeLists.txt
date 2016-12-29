cmake_minimum_required(VERSION 3.0.0)

set(CMAKE_CXX_STANDARD "14")

if(CMAKE_BUILD_TYPE STREQUAL "Debug")
    set(CMAKE_CXX_FLAGS "-g")
endif()

project(xox)

file(GLOB srcs "${CMAKE_SOURCE_DIR}/src/*.cpp")
include_directories("${CMAKE_SOURCE_DIR}/include")



add_executable(xox ${srcs})
target_link_libraries(xox )