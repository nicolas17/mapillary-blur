cmake_minimum_required(VERSION 2.8.12)

project(mapillary-blur CXX)

# Find includes in corresponding build directories
set(CMAKE_INCLUDE_CURRENT_DIR ON)
# Instruct CMake to run moc automatically when needed.
set(CMAKE_AUTOMOC ON)

# Find the QtWidgets library
find_package(Qt5Widgets)

add_executable(mapillary-blur WIN32 main.cpp)

target_link_libraries(mapillary-blur Qt5::Widgets)
