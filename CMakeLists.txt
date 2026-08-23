cmake_minimum_required(VERSION 4.4)

project(easyEngine)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/CMake")

find_package(slang CONFIG HINTS "$ENV{VULKAN_SDK}/lib/cmake")

add_executable(Engine main.cpp)