cmake_minimum_required(VERSION 3.10)

project(OpticalFlow)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenCV REQUIRED)

add_executable(optical_flow main.cpp)

target_include_directories(optical_flow PRIVATE ${OpenCV_INCLUDE_DIRS})

target_link_libraries(optical_flow PRIVATE ${OpenCV_LIBS})

