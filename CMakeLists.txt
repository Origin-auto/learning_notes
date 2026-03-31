# 指定最低 CMake 版本
cmake_minimum_required(VERSION 3.10)

# 项目名称
project(learning)

# 指定 C++ 标准（例如 C++17）
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 添加可执行文件
# 参数解释：生成的程序名  源文件路径
add_executable(${PROJECT_NAME} src/main.cpp)