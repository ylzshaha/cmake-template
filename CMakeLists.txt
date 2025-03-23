cmake_minimum_required(VERSION 3.2)

project(cmake-project-template)

set(CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_STANDARD 20)
set(EXPORT_COMPILE_COMMANDS ON)

set(CMAKE_INSTALL_PREFIX ${PROJECT_SOURCE_DIR})

set(PROJECT_INSTALL_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/include)
set(PROJECT_INSTALL_BIN_DIR ${PROJECT_SOURCE_DIR}/bin)
set(PROJECT_INSTALL_LIB_DIR ${PROJECT_SOURCE_DIR}/lib)

set(_HEADERS_DIR ${PROJECT_SOURCE_DIR}/src/division)

include_directories(${PROJECT_INSTALL_INCLUDE_DIR})
include_directories(${PROJECT_HEADERS_DIR})

add_subdirectory(src)
add_subdirectory(test)


