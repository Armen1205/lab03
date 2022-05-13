# lab03

CMAKE система используется для автоматической сборки проекта по его исходному коду. При этом сама система не занимается самой сборкой, она использует различные версии make. 

задание 1:
 cmake_minimum_required(VERSION 3.4)
 project(formatter)
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)  
 add_library(formatter STATIC ${CMAKE_CURRENT_SOURCE_DIR}/formatter.cpp)
 add_executable(formatter ${CMAKE_CURRENT_SOURCE_DIR}/formatter.cpp)
 target_link_libraries(formatter formatter_lib1)
 EOF
