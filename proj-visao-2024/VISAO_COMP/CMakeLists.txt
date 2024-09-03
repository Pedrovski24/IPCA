cmake_minimum_required(VERSION 3.5)

project(VISAO_COMP)
set(OpenCV_DIR C:/opencv/build/x64/vc16/lib)

set(SOURCES
    trab.cpp
    vc.c
    vc.h
)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(VISAO_COMP ${SOURCES})

target_link_libraries(VISAO_COMP ${OpenCV_LIBS})