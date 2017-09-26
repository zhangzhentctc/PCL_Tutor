cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(don_segmentation)

find_package(PCL 1.7 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (example_difference_of_normals example_difference_of_normals.cpp)
target_link_libraries (example_difference_of_normals ${PCL_LIBRARIES})
