cmake_minimum_required(VERSION 3.4.1)
project(AwesomeLibrary)

set (CMAKE_VERBOSE_MAKEFILE ON)
set (CMAKE_CXX_STANDARD 11)

add_library(react-native-awesome-library            SHARED
            ../cpp/react-native-awesome-library.cpp
            cpp-adapter.cpp
)

# Specifies a path to native header files.
include_directories(
            ../cpp
)
