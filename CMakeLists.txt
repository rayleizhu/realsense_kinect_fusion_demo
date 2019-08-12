cmake_minimum_required(VERSION 3.10)
project(realsense_kinfu)

set(CMAKE_CXX_STANDARD 11)

set(CMAKE_PREFIX_PATH /home/rayleizhu/miniconda3/envs/opencv4/)

find_package(OpenCV REQUIRED)
message(STATUS "OpenCV library status:")
message(STATUS "    version: ${OpenCV_VERSION}")
message(STATUS "    libraries: ${OpenCV_LIBS}")
message(STATUS "    include path: ${OpenCV_INCLUDE_DIRS}")

set(DEPENDENCIES realsense ${OpenCV_LIBS})

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(realsense_kinfu main.cpp)
target_link_libraries(realsense_kinfu realsense ${DEPENDENCIES})
