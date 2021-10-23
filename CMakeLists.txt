project(Calender)
cmake_minimum_required(VERSION 3.4.1)
set(CMAKE_CXX_STANDARD 17)

set(TARGET_NAME Calendar)
set(EXECUTABLE_OUTPUT_PATH  ${CMAKE_CURRENT_SOURCE_DIR}/bin)
set(LIBRARY_OUTPUT_PATH     ${CMAKE_CURRENT_SOURCE_DIR}/lib)
set(CMAKE_ROOT_PATH         ${CMAKE_CURRENT_SOURCE_DIR})

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -g")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -g")

set(SRC_PATH                ${CMAKE_SOURCE_DIR}/src)

include(${CMAKE_CURRENT_SOURCE_DIR}/cmake/toolchain.cmake)

add_executable(${TARGET_NAME})
add_subdirectory(${SRC_PATH})
