# cmake_minimum_required(VERSION 2.8)
# project(libhello)

# file(GLOB_RECURSE ROOT_SRC_FILES
#     ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c
#     ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cc
#     ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp
#     )

# file(GLOB INCLUDE_FILES
#     ${CMAKE_CURRENT_SOURCE_DIR}/include/seeta/*.h
#     ${CMAKE_CURRENT_SOURCE_DIR}/include/seeta/*.hh
#     ${CMAKE_CURRENT_SOURCE_DIR}/include/seeta/*.hpp
#     )

# set_property(
#     TARGET
#         ${PROJECT_NAME}
#     PROPERTY
#         PUBLIC_HEADER ${INCLUDE_FILES}
# )

add_library(hello STATIC hello.cpp)
# list(APPEND SRC_FILES ${ROOT_SRC_FILES})
# add_library(${PROJECT_NAME} ${SRC_FILES})