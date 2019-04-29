cmake_minimum_required(VERSION 3.13.3)
project (testing-catch2)

# cmake .. -G "MinGW Makefiles"
# mingw32-make

include_directories(include)
include_directories(C:/Catch2)
#file(GLOB SOURCES "include/game/*.cpp")
set(SOURCES 
    010-TestCase.cpp
    C:/Catch2/catch.hpp
)

add_executable(Testing-Catch2 ${SOURCES})