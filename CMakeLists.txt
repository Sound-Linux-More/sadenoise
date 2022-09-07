cmake_minimum_required(VERSION 2.8)
project(sadenoise LANGUAGES C)
set(CMAKE_POSITION_INDEPENDENT_CODE ON)
SET(CMAKE_BUILD_TYPE "Release")

include_directories(src)

add_executable(${PROJECT_NAME} src/main.c)

target_link_libraries(${PROJECT_NAME} -lm)
