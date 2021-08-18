# Minimum CMake vesion
cmake_minimum_required(VERSION 3.21.1)

# Project
project(Test CXX)

# Executable 
add_executable(${PROJECT_NAME} Main.cpp)

# Add SFML
add_subdirectory(extlibs/SFML)

# Link SFML
target_link_libraries(${PROJECT_NAME} PRIVATE sfml-window sfml-system sfml-graphics)
