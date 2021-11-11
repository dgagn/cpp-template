cmake_minimum_required(VERSION 3.20)
project(cpp_work)

set(CMAKE_CXX_STANDARD 23)
set(SOURCE_FILES main.cpp)
add_executable(sources_run ${SOURCE_FILES})

include_directories(src)
add_subdirectory(src)

target_link_libraries(sources_run sources_lib)

add_subdirectory(tests)
