cmake_minimum_required(VERSION 3.16)
project(test_package)

find_package(Eigen3 REQUIRED CONFIG)

add_executable(${PROJECT_NAME} test_package.cpp)
target_link_libraries(${PROJECT_NAME} Eigen3::Eigen)
