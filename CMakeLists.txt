cmake_minimum_required(VERSION 3.8.2)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(wxWidgets_USE_DEBUG 1)
set(wxWidgets_USE_STATIC 1)

add_subdirectory(base)
add_subdirectory(gow)
add_subdirectory(app)
