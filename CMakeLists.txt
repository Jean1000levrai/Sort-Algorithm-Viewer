cmake_minimum_required(VERSION 3.16)

project(application)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_C_EXTENSIONS OFF)

# find sdl3
find_package(SDL3 REQUIRED CONFIG)

# the source files
file(GLOB SRC_FILES src/*.c)

add_executable(application ${SRC_FILES})

# include
target_include_directories(application PRIVATE include)

# sdl3
target_link_libraries(application PRIVATE SDL3::SDL3)