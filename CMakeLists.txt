cmake_minimum_required(VERSION 3.0.0)
project(gputest)
set(CMAKE_CXX_STANDARD 20)
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(gputest main.cpp)
target_link_libraries(gputest ${OpenCV_LIBS})