cmake_minimum_required(VERSION 3.25)
project(lib C)

set(CMAKE_C_STANDARD 11)

add_library(digger_curl INTERFACE)
target_include_directories(digger_curl INTERFACE curl/include)
target_sources(digger_curl INTERFACE curl/src)