cmake_minimum_required(VERSION 3.11.0)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARd_REQUIRED ON)

project(
        PSsimplesafeint
        VERSION 0.1.0
        DESCRIPTION "A C++20 implementation of safe (wrap around) integers following MISRA C++ rules."
        LANGUAGES CXX
)

add_library(${PROJECT_NAME} INTERFACE)
target_include_directories(${PROJECT_NAME}
        INTERFACE
                "${PROJECT_SOURCE_DIR}/include"
)
