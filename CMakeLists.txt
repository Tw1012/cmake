cmake_minimum_required(VERSION 3.25 FATAL_ERROR)

project(cmake
    VERSION         0.0.1
    DESCRIPTION     "Thy's CMake demo"
    HOMEPAGE_URL    "https://github.com/Tw1012/cmake"
    LANGUAGES       c cxx
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(Buildinfo)

add_subdirectory(external)

add_subdirectory(docs)

add_subdirectory(test)

add_subdirectory(src)

add_subdirectory(packaging)