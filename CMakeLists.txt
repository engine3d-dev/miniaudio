cmake_minimum_required(VERSION 3.27)
project(miniaudio LANGUAGES C CXX)

build_library(
    DIRECTORIES src
)

generate_compile_commands()

target_include_directories(${PROJECT_NAME} PUBLIC ./)
target_include_directories(${PROJECT_NAME} PRIVATE audio audio/internal)