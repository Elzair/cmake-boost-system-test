cmake_minimum_required(VERSION 3.3)

project(test_system)

add_subdirectory(libs)

add_executable(test_system test.cpp)

target_link_libraries(test_system
  boost::assert
  boost::config
  boost::core
  boost::predef
  boost::system)
