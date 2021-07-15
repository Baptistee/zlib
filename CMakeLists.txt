cmake_minimum_required(VERSION 3.5)

project(zlib)

file(GLOB
        ZLIB_SRC
        zlib/*.c
        )

add_library(${PROJECT_NAME}
        STATIC
        ${ZLIB_SRC}
        )

target_include_directories(${PROJECT_NAME}
        PUBLIC
        zlib
        )
