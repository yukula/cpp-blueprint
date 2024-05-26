cmake_minimum_required(VERSION 3.28)

project(cpp-blueprint CXX)
include_directories(include)


find_package(fmt REQUIRED)
add_executable(${PROJECT_NAME})
target_sources(${PROJECT_NAME}
  PRIVATE
    src/main.cpp
)
target_link_libraries(${PROJECT_NAME} fmt::fmt)


find_package(doctest REQUIRED COMPONENTS system)
add_executable(mainTest tests/mainTest.cpp)
target_link_libraries(mainTest fmt::fmt doctest::doctest)


enable_testing()
add_test(NAME AllTests COMMAND mainTest)
