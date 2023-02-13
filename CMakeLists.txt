cmake_minimum_required(VERSION 3.24)
project(gas77 C)

set(CMAKE_C_STANDARD 23)

add_executable(gas77 main.c)

if(WIN32)
    target_link_libraries(gas77 wsock32 ws2_32)
endif()