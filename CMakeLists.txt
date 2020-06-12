cmake_minimum_required(VERSION 3.4.0)
project(CmakeTest VERSION 0.1.0)

message("======")
add_subdirectory(set)
add_subdirectory(message)
add_subdirectory(grammer)
add_subdirectory(properties)
add_subdirectory(function)

include(CTest)
enable_testing()

add_executable(CmakeTest main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)