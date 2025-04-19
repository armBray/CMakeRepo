cmake_minimum_required(VERSION 3.13)
project(testsome)
add_executable(testsome main.cpp)
target_link_directories(testsome PRIVATE ${CMAKE_SOURCE_DIR}/../1_SomeLibDemo/cpp/build) #target_link_directories available only on cmake VERSION 3.13 - target_link_directories($(executable_where_to_link_the_library $(path_to_lib".a""))) - PRIVATE is used to not expose the library
target_link_libraries(testsome mearlymath)

# if mearlymath lib is installed locally, target_link_directories() is not needed