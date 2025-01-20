cmake_minimum_required(VERSION 3.0)
project(riscvsim)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(include)
file(GLOB SOURCES "src/*.cpp")

add_executable(riscvsim ${SOURCES})

enable_testing(tests)
add_subdirectory(tests)

