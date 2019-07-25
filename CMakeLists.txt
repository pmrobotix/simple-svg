#project (simple-svg)
#cmake_minimum_required(VERSION 2.8)

#add_executable(simple_svg main_1.0.0.cpp simple_svg_1.0.0.hpp)

#set_property(TARGET simple_svg PROPERTY CXX_STANDARD 11)

                     
#if(MSVC)
#   add_definitions(/D_CRT_SECURE_NO_WARNINGS)
#   add_definitions(/D_SCL_SECURE_NO_WARNINGS)
#   add_definitions(/DNOMINMAX)
#endif(MSVC)



set(APP_NAME simple-svg)
project(${APP_NAME})
cmake_minimum_required(VERSION 2.8)
add_library(${PROJECT_NAME} STATIC main_1.0.0.cpp simple_svg_1.0.0.hpp)
#set(CMAKE_BUILD_TYPE LibCMAKE)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
