cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(openni_tracking)

find_package(PCL 1.7 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (openni_tracking openni_tracking.cpp)
target_link_libraries (openni_tracking ${PCL_LIBRARIES})
