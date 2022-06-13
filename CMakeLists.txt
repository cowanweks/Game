cmake_minimum_required(VERSION 3.21)

project(GAME)
# Use C++ 17 standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Add Compiler flags
set(CMAKE_CXX_FLAGS "-g -Wall -Werror")
file(GLOB CPP_SOURCE
    "${PROJECT_SOURCE_DIR}/src/*.cpp"
    "${PROJECT_SOURCE_DIR}/src/*/*.cpp"
    )

include_directories(${PROJECT_SOURCE_DIR}/include)

add_executable(main ${CPP_SOURCE})