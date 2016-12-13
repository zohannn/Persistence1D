cmake_minimum_required(VERSION 2.8)
set(CMAKE_CXX_FLAGS "-g -Wall -std=c++11")

set(PROJECT_NAME Persistence1D)
project (${PROJECT_NAME})

set(CMAKE_BUILD_TYPE Release)


add_library(${PROJECT_NAME} SHARED src/persistence1d_driver.cpp include/persistence1d.hpp)
install(TARGETS ${PROJECT_NAME} DESTINATION ${CMAKE_CURRENT_SOURCE_DIR}/lib)
