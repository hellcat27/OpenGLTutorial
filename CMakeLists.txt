cmake_minimum_required(VERSION 3.28)
project(OpenGLTutorials)

set(CMAKE_CXX_STANDARD 17)
add_subdirectory(GLFW)
link_directories(GLFW)
#add_subdirectory(include)
link_directories(include)


include_directories(GLFW)
include_directories(include)

add_executable(OpenGLTutorials main.cpp
        include/src/glad.c)
target_link_libraries(OpenGLTutorials glfw)
#target_link_libraries(OpenGLTutorials ${OpenGLLibs})
