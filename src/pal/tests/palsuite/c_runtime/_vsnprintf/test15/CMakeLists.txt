cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test15.c
)

add_executable(paltest_vsnprintf_test15
  ${SOURCES}
)

add_dependencies(paltest_vsnprintf_test15 CoreClrPal)

target_link_libraries(paltest_vsnprintf_test15
  pthread
  m
  CoreClrPal
)
