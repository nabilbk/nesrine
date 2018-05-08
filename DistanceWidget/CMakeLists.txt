
cmake_minimum_required(VERSION 2.8)
 
PROJECT(DistanceWidget)
 
find_package(VTK REQUIRED)
include(${VTK_USE_FILE})
 
add_executable(DistanceWidget MACOSX_BUNDLE DistanceWidget.cxx )
 
target_link_libraries(DistanceWidget ${VTK_LIBRARIES})
