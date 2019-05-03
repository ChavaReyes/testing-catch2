cmake_minimum_required(VERSION 3.13.3)
project (testing-catch2)

# cmake .. -G "MinGW Makefiles"
# mingw32-make

include_directories(C:/Catch2)

add_executable(Test1 010-TestCase.cpp C:/Catch2/catch.hpp)
add_executable(Test2 100-Fix-Section.cpp C:/Catch2/catch.hpp)
add_executable(Test3 120-Bdd-ScenarioGivenWhenThen.cpp C:/Catch2/catch.hpp)

#add_library(Catch2Lib INTERFACE)
#target_include_directories(Catch2Lib INTERFACE C:/Catch2)

#set(APP_SOURCES 
#    010-TestCase.cpp
#    100-Fix-Section.cpp
#    120-Bdd-ScenarioGivenWhenThen.cpp
#)

#foreach(testsourcefile ${APP_SOURCES})
#    string(REPLACE ".cpp" "" testname ${testsourcefile})
#    add_executable(${testname} ${testsourcefile})
#    target_link_libraries(${testname} Catch2Lib)
#endforeach(testsourcefile ${APP_SOURCES})