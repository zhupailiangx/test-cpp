
cmake_minimum_required(VERSION 2.8)
Project(test)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
add_executable(test_hello src/main.cpp src/hello.cpp)