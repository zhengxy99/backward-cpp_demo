# backward-cpp_demo
首先安装lib  apt-get install libdw-dev 
注意在CMakeList.txt中添加
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g")
注意对dw的链接
target_link_libraries(test dw)
