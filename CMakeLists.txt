cmake_minimum_required(VERSION 2.6)
project (threadpool)

find_package (Threads)
SET (CMAKE_CXX_COMPILER             "/usr/bin/clang++")
set (CMAKE_CXX_STANDARD 11)
set (CMAKE_CXX_FLAGS -g)
add_executable(threadpool example.cpp)
target_link_libraries(threadpool ${CMAKE_THREAD_LIBS_INIT})

