cmake_minimum_required(VERSION 3.10)

project(HelloWorld)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_OSX_ARCHITECTURES x86_64)

find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

add_executable(HelloWorld main.cpp)
target_link_libraries(HelloWorld sfml-graphics sfml-window sfml-system)