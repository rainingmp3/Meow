cmake_minimum_required(VERSION 3.31.0 FATAL_ERROR)
set(PROJECT_NAME Meow)
project(${PROJECT_NAME})

add_executable(${PROJECT_NAME} src/main.cpp)

add_subdirectory(external/glfw)
target_link_libraries(${PROJECT_NAME} glfw)