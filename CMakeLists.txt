#项目名称
#PROJECT(HELLOWORLD)
 
#定义变量
#SET(SRC_LIST helloworld.cpp)
 
#打印用户的一些信息
#MESSAGE(STATUS "This is BINARY dir " ${HELLOWORLD_BINARY_DIR})
#MESSAGE(STATUS "This is SOURCE dir "${HELLOWORLD_SOURCE_DIR})
 
#生成可执行文件s
#ADD_EXECUTABLE(helloworld ${SRC_LIST})

cmake_minimum_required(VERSION 3.10)
project(cppproject)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g")

add_subdirectory(./backward-cpp)


add_executable(test main.cpp ${BACKWARD_ENABLE} ${ARGN})
target_link_libraries(test dw)







