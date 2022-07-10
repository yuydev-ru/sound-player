cmake_minimum_required(VERSION 3.20)
project (sound-player)
set (CMAKE_CXX_STANDARD 17)

add_executable (SoundPlayer Source/main.cpp)

add_subdirectory (Dependencies)

target_link_libraries (SoundPlayer LINK_PRIVATE glfw)
target_link_libraries (SoundPlayer LINK_PRIVATE imgui)

