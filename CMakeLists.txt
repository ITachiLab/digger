cmake_minimum_required(VERSION 3.25)
project(digger C)

set(CMAKE_C_STANDARD 11)

add_subdirectory(lib)

add_executable(digger main.c)

target_link_libraries(digger INTERFACE digger_curl)
target_link_libraries(digger PUBLIC curl)