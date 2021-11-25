cmake_minimum_required(VERSION 3.16)
project(HydroMini)

set(CMAKE_CXX_STANDARD 17)
find_package (Eigen3 3.3 REQUIRED NO_MODULE)
add_compile_options(-std=c++17 -O2 -g -Wall -Wextra -pedantic -Wmissing-include-dirs -Wformat=2 -Wunused -Wcast-align -Wnon-virtual-dtor -Woverloaded-virtual)


add_executable(HydroMini src/main.cpp include/NetworkSolve.h)

target_link_libraries(HydroMini Eigen3::Eigen)
