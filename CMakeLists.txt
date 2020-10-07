cmake_minimum_required(VERSION 3.17)
project(saper)

find_package(SFML CONFIG REQUIRED system window graphics)

set(CMAKE_CXX_STANDARD 20)

add_compile_options(/W3 /Za /TP /permissive-)

add_executable(saper main.cpp)
target_link_libraries(saper sfml-graphics sfml-audio sfml-system)
