cmake_minimum_required(VERSION 2.8.9)

get_filename_component(DIR_NAME "${CMAKE_CURRENT_LIST_DIR}" NAME)
project(${DIR_NAME})

set(CMAKE_CXX_STANDARD 17)

include_directories(inc/)

set(HELLO_HEADER_FILES
        inc/Test.hpp)
set(HELLO_SOURCE_FILES
        src/Test.cpp)
set(MAIN_FILE
        src/main.cpp)

add_executable(${PROJECT_NAME}
               ${HELLO_HEADER_FILES}
               ${HELLO_SOURCE_FILES}
               ${MAIN_FILE})
