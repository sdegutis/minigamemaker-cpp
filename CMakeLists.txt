cmake_minimum_required(VERSION 3.31)

project(HelloWorld)

find_package(SDL3 CONFIG REQUIRED)

add_executable(HelloWorld src/helloworld.cpp)

target_link_libraries(HelloWorld PRIVATE SDL3::SDL3)
set_property(TARGET HelloWorld PROPERTY WIN32_EXECUTABLE TRUE)
