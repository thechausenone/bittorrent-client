cmake_minimum_required(VERSION 3.13)

project(
  divvy
  VERSION 1.0
  LANGUAGES CXX)

set(SOURCE_FILES
    HelloWorld.h
    HelloWorld.cpp
)

add_library(HelloWorld SHARED STATIC ${SOURCE_FILES})

install(TARGETS HelloWorld DESTINATION ${DIVVY_INSTALL_LIB_DIR})
install(FILES HelloWorld.h DESTINATION ${DIVVY_INSTALL_INCLUDE_DIR})
