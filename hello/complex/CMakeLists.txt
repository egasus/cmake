cmake_minimum_required(VERSION 2.8)
project(sayhello)
add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} hello)

include_directories(./hello)
add_subdirectory(hello)