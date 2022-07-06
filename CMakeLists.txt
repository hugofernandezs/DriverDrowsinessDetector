# Project compiler settings
cmake_minimum_required(VERSION 3.16)
set(CMAKE_CXX_STANDARD 20)

# Project settings
set(PROJECT DriverDrowsinessDetector)
project(${PROJECT})

# Project files
file(GLOB_RECURSE HEADERS lib/*)
file(GLOB_RECURSE SOURCES src/*)

# Project build configuration
add_executable(${PROJECT} ${HEADERS} ${SOURCES})