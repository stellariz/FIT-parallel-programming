cmake_minimum_required(VERSION 3.17)
project(lab4 C)

set(CMAKE_C_STANDARD 99)

find_package(MPI REQUIRED)
include_directories(${MPI_INCLUDE_PATH})

set(CMAKE_C_COMPILER mpicc)

add_executable(lab4 main.c)