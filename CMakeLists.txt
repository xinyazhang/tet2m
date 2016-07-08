cmake_minimum_required(VERSION 3.0)

project(tet2m)
set (tet2m_VERSION_MAJOR 0)
set (tet2m_VERSION_MINOR 1)

find_package(Eigen3 REQUIRED)
include_directories(${IGL_INCLUDE_DIR})
include_directories(${EIGEN3_INCLUDE_DIR})

AUX_SOURCE_DIRECTORY(src SRC)
ADD_EXECUTABLE(tet2m ${SRC})
