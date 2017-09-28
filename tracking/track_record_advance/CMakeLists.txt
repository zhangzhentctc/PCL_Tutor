cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(track_record_advance)

find_package(PCL 1.7 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (track_record_advance track_record_advance.cpp)
target_link_libraries (track_record_advance ${PCL_LIBRARIES})
