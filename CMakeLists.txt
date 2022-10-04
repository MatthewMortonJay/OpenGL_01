cmake_minimum_required(VERSION 3.23)
project(OpenGL_01)

set(CMAKE_CXX_STANDARD 14)

add_executable(OpenGL_01 ${PROJECT_SOURCE_DIR}/main.cpp ${PROJECT_SOURCE_DIR}/src/glad.c)

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)
target_link_libraries(OpenGL_01 ${PROJECT_SOURCE_DIR}/lib/glfw3.dll)