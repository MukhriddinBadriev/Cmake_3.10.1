cmake_minimum_required (VERSION 3.8)

add_executable (my_first_cmake_project "my_first_cmake_program.cpp" "my_first_cmake_project.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET my_first_cmake_project PROPERTY CXX_STANDARD 20)
endif()