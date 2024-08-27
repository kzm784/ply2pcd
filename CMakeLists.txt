cmake_minimum_required(VERSION 3.0.2)
project(ply2pcd)

find_package(PCL 1.7 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable(ply2pcd src/ply2pcd.cpp)
target_link_libraries(ply2pcd ${PCL_LIBRARIES})

