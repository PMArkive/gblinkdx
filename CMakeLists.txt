cmake_minimum_required(VERSION 3.8)
project(gblinkdx)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        gblinkdl.cpp
        typedefs.h
        ppgb.c
        ppgb.h)

set(CMAKE_CXX_FLAGS "-static-libgcc -static-libstdc++ -s")

add_executable(gblinkdx ${SOURCE_FILES})