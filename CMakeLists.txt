set(CMAKE_VERBOSE_MAKEFILE 1)
cmake_minimum_required(VERSION 3.0)

# EXECUTABLE FILE
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
add_executable(main.out main.cpp)

# SUBDIRECTORIES
add_subdirectory(lib)
target_link_libraries(main.out Lib)
