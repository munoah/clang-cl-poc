# CMakeList.txt : Top-level CMake project file, do global configuration
# and include sub-projects here.
#
cmake_minimum_required (VERSION 3.13)

project ("cmake")
# Include sub-projects.
include(conan.cmake)
conan_cmake_run(REQUIRES boost/1.71.0@conan/stable
				BASIC_SETUP 
				CMAKE_TARGETS
				PROFILE default
				BUILD missing)
add_subdirectory ("cmake")
