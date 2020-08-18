cmake_minimum_required(VERSION 3.17)
project(RoadInfoManage C)

set(CMAKE_C_STANDARD 11)

add_executable(RoadInfoManage src/main.c)
set_target_properties(RoadInfoManage PROPERTIES COMPILE_FLAGS "-Wno-unused-result -fsanitize=address")
target_link_libraries(RoadInfoManage -fsanitize=address)
