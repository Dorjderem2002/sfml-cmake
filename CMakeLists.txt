cmake_minimum_required(VERSION 3.0)
project(program)

set (CMAKE_CXX_STANDARD 17)
find_package(SFML 2.5.1 COMPONENTS audio graphics window system REQUIRED)

set(SOURCES
    main.cpp
    )

add_executable(program ${SOURCES})

target_link_libraries(program sfml-audio sfml-graphics sfml-window sfml-system)