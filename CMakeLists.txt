cmake_minimum_required(VERSION 3.20)
project(SysCompEX3 C ASM)

set(CMAKE_C_STANDARD 99)

set(GCC_COVERAGE_COMPILE_FLAGS "-no-pie")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}")

add_executable(SysCompEX3 main.c run_main.s func_select.s pstring.s)
