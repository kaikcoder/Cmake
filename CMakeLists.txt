cmake_minimum_required(VERSION 3.29.0)  # 指定 cmake 的最低版本
project(planning)  # 设置一个工程名
set(CMAKE_CXX_STANDARD 11)  # 选择 C++11 以上

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)  # 设置 C++ 可执行文件的路径
aux_source_directory(./ SRC_LISTS)  # 获取当前目录的所有 cpp 文件

add_executable(planning_main ${SRC_LISTS})  # 生成可执行文件
