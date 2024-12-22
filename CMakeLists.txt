cmake_minimum_required(VERSION 3.26)
project(opengl_demo)

set(CMAKE_CXX_STANDARD 17)

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)

add_executable(opengl_demo main.cpp src/glad.c)

target_link_libraries(opengl_demo ${PROJECT_SOURCE_DIR}/lib/glfw3.dll)