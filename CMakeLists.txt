cmake_minimum_required(VERSION 3.6)
project(mesh-io-DSC)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(2D-DSC)
add_subdirectory(DSC)
add_subdirectory(GEL)
add_subdirectory(mesh-io-2D)
add_subdirectory(mesh-io-3D)

aux_source_directory(interface SRC)
add_executable(dsc-mesh ${SRC})
