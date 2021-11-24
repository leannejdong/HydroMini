cmake_minimum_required(VERSION 3.20)
project(HydroMini)

set(CMAKE_CXX_STANDARD 17)
find_package (Eigen3 3.3 REQUIRED NO_MODULE)

add_executable(HydroMini src/main.cpp include/NetworkSolve.h)

target_link_libraries(HydroMini Eigen3::Eigen)
