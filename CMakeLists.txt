cmake_minimum_required(VERSION 3.1)
project(deadlock)
set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_C_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g")
add_executable(deadlock deadlock.c)
target_link_libraries(deadlock pthread dl)




