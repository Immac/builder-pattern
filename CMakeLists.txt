cmake_minimum_required(VERSION 3.11.2)
project(cpp-template VERSION 1.0.0.0 LANGUAGES CXX)
#message(${CMAKE_CURRENT_SOURCE_DIR})
add_executable(Template ../src/main.cpp )
set_target_properties(Template PROPERTIES RUNTIME_OUTPUT_DIRECTORY bin/${CMAKE_BUILD_TYPE})
target_include_directories(Template
PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/src
)

