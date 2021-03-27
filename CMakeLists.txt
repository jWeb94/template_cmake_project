cmake_minimum_required(VERSION 3.0)
project(test_project_cmake)

add_executable(my_exec src/main.cpp)

target_include_directories(my_exec PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>)