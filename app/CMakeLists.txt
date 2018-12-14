cmake_minimum_required(VERSION 3.8.2)

file(GLOB SRC_FILES "*.cpp")

if(WIN32)
	add_executable(wxcmake WIN32 ${SRC_FILES})
else()
	add_executable(wxcmake ${SRC_FILES})
endif()

target_link_libraries(wxcmake 3rdparty::wx::net 3rdparty::wx::core 3rdparty::wx::base)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

