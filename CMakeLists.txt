cmake_minimum_required(VERSION 3.22.2)

project(cf_fat C)

add_library(${PROJECT_NAME} STATIC
    mem-cf.c
    mem-cf.h
    mem-ffs.c
    mem-ffs.h
    mem-types.h
)

target_include_directories(${PROJECT_NAME}
    PUBLIC .
)
