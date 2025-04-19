cmake_minimum_required(VERSION 2.8)
project(Trim)
add_executable(trim main.cpp) #($(name_to_call_the_exec) $(reference_to_source))
install(TARGETS trim DESTINATION bin) #if you want to install locally (TARGETS $(name_to_call_the_exec) DESTINATION $(path)) by default $(path)=usr/local/bin