# Specify the minimum version of CMake required
cmake_minimum_required(VERSION 3.10)

# Set the project name and version
project(HelloWorld VERSION 0.0.1)

# Specify the C++ standard to use (will update in march with ubuntu 26.04)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Add an executable target
# Usage: add_executable(executable_name source_files)
add_executable(hello_world test.cpp)