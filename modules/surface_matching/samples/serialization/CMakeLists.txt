cmake_minimum_required (VERSION 2.6)

include_directories(
  "${CMAKE_SOURCE_DIR}/../../../../../opencv/include/"
  "${CMAKE_SOURCE_DIR}/../../include/"
)

link_directories(
  "${CMAKE_SOURCE_DIR}/../../../../../opencv/build/lib/"
)

project (Serialization)
add_executable(serialization serialization.cpp)
target_link_libraries(serialization opencv_core opencv_surface_matching)