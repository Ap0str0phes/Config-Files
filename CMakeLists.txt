set(name "Shell")

cmake_minimum_required(VERSION 3.28)

project(${name})

file(GLOB_RECURSE SRC_FILES src/*.cpp)

add_executable(${name} main.cpp ${SRC_FILES})

target_include_directories(${name} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
