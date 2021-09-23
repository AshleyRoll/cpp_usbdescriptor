cmake_minimum_required(VERSION 3.21)
project(usbdescriptors)

set(CMAKE_CXX_STANDARD 20)

add_executable(usbdescriptors main.cpp)

target_include_directories(usbdescriptors
        PUBLIC
        $<BUILD_INTERFACE:${CMAKE_SOURCE_DIR}/include>
        $<BUILD_INTERFACE:${CMAKE_BINARY_DIR}/include>
        $<INSTALL_INTERFACE:include>
        )
