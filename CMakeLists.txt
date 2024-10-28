cmake_minimum_required(VERSION 3.10)

# 设置项目名称
project(MyCppProject)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 添加可执行文件
add_executable(MyCppProject
    src/main.cpp
    src/task1.cpp
    # 添加其他源文件
)

# 包含头文件目录
target_include_directories(MyCppProject PRIVATE
    ${PROJECT_SOURCE_DIR}/include
)