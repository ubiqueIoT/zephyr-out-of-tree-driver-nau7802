cmake_minimum_required(VERSION 3.20.0)

list(APPEND ZEPHYR_EXTRA_MODULES "${CMAKE_CURRENT_SOURCE_DIR}/drivers")

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(nau7802-test-delete-me)

target_sources(app PRIVATE src/main.c)
