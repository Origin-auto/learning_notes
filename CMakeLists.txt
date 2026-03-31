cmake_minimum_required(VERSION 3.15)
project(learning_notes LANGUAGES CXX)

# 强制所有输出到 build 目录
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

# 自动收集 src 下所有 .cpp 文件
file(GLOB SOURCES "src/*.cpp")

# 创建可执行文件
add_executable(${PROJECT_NAME} ${SOURCES})

# 可选：指定 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)