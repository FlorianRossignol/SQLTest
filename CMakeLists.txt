cmake_minimum_required (VERSION 3.30)
project(SQL)


set (CMAKE_CXX_STANDARD 20)
set (CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt6 REQUIRED COMPONENTS Core)
qt_standard_project_setup()

qt_add_executable(SQL
    main.cpp
)

target_link_libraries(SQL PRIVATE Qt6::CORE)
