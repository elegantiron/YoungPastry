cmake_minimum_required(VERSION 3.30)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin/package)
include(FetchContent)
FetchContent_Declare(
    pegtl
    GIT_REPOSITORY https://github.com/taocpp/pegtl.git
    GIT_TAG 3.2.8
    GIT_SHALLOW ON
    SYSTEM
    EXCLUDE_FROM_ALL
)
FetchContent_MakeAvailable(
    pegtl
)
project(YoungPastry)

add_subdirectory(libyunpa)