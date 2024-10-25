cmake_minimum_required(VERSION 3.10)

project(BST)

add_library(BST INTERFACE)

target_include_directories(BST INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

target_compile_features(BST INTERFACE cxx_std_17)

add_subdirectory(examples)

add_subdirectory(tests)
