cmake_minimum_required(VERSION 3.8.2)

set(wxBUILD_SHARED FALSE)

add_subdirectory(wxWidgets)

add_library(3rdparty::wx::net ALIAS net)
add_library(3rdparty::wx::base ALIAS base)
add_library(3rdparty::wx::core ALIAS core)
