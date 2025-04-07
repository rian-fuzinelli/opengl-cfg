cmake_minimum_required(VERSION 3.21)
project(project_opengl)

set(CMAKE_CXX_STANDARD 17)

find_package(glfw3 CONFIG REQUIRED)
find_package(glad CONFIG REQUIRED)
add_executable(project_opengl main.cpp)

target_link_libraries(project_opengl PRIVATE glfw glad::glad)
