project(zlib)

include_directories(zlib)

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
