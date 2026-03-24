cmake_minimum_required(VERSION 3.21)
project(simple-svg LANGUAGES CXX)

add_library(simple-svg STATIC
    simple_svg_1.0.0.cpp
)

target_include_directories(simple-svg PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)
