add_executable (cmake "cmake.cpp" "cmake.h")
target_link_libraries(cmake PRIVATE CONAN_PKG::boost)
