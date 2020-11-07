cmake_minimum_required(VERSION 3.13)

project(
  divvy
  VERSION 1.0
  LANGUAGES CXX)

add_subdirectory(HelloWorld)
set(SOURCE_FILES main.cpp)

add_executable(divvy ${SOURCE_FILES})
target_link_libraries(divvy HelloWorld)
install(TARGETS divvy DESTINATION ${DIVVY_INSTALL_BIN_DIR})
