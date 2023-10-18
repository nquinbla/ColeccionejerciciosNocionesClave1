cmake_minimum_required(VERSION 3.26)
project(ejerciciosnocionesclave1_2)

set(CMAKE_CXX_STANDARD 17)

add_executable(main main.cpp)
add_library(persona STATIC persona.cpp)
add_library(estudiante STATIC estudiante.cpp
        Persona.cpp
        Persona.h
        Estudiante.cpp
        Estudiante.h)

target_link_libraries(main persona estudiante)
