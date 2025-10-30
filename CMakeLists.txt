cmake_minimum_required(VERSION 3.18)

project(vulkan-tutorial)

add_executable(app)

target_sources(app
    PRIVATE
        src/main.cpp
)


find_package(glfw3 REQUIRED)
target_link_libraries(app vulkan glfw)