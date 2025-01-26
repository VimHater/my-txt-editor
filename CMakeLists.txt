# Minimum CMake version required
cmake_minimum_required(VERSION 3.15)

# Project name and version
project(my-txt-editor VERSION 1.0)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Include directories
include_directories(include)

# Find all source files
file(GLOB_RECURSE SOURCES "src/*.cpp")

# Create the executable
add_executable(${PROJECT_NAME} ${SOURCES})
