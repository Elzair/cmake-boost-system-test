if(APPLE)
  cmake_minimum_required(VERSION 2.8.11 FATAL_ERROR)
else()
  cmake_minimum_required(VERSION 2.8.7 FATAL_ERROR)
endif()

project(test_system)

add_subdirectory(libs)

add_executable(test_system test.cpp)

target_link_libraries(test_system boost_predef boost_config boost_assert boost_core boost_system)
