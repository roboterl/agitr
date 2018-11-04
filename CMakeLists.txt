cmake_minimum_required(VERSION 2.8.3)
project(agitr)

find_package(catkin REQUIRED COMPONENTS
    roscpp
    )

catkin_package()

include_directories(include ${catkin_INCLUDE_DIRS})

add_executable(hello_node src/hello.cpp)
target_link_libraries(hello_node ${catkin_LIBRARIES})
