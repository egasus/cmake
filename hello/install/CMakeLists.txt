cmake_minimum_required(VERSION 2.8)
project(hello)

add_executable(hello main.cpp)

# set( CMAKE_INSTALL_PREFIX "${CMAKE_BINARY_DIR}/install" CACHE PATH "Install path prefix." FORCE)
set(CMAKE_INSTALL_PREFIX "${CMAKE_SOURCE_DIR}/build/bin/")
install(TARGETS hello RUNTIME DESTINATION ${CMAKE_INSTALL_PREFIX})

