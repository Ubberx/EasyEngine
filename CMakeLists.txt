cmake_minimum_required(VERSION 4.4)

project(easyEngine)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/CMake")

find_package(slang CONFIG HINTS "$ENV{VULKAN_SDK}/lib/cmake")

find_package(glm CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
find_package(tinyobjloader CONFIG REQUIRED)
find_package(stb CONFIG REQUIRED)

add_executable(Engine main.cpp)