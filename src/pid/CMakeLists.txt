cmake_minimum_required(VERSION 3.0.2)
project(pid)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  sensor_msgs
  nav_msgs
  geometry_msgs
  std_msgs
  gazebo_msgs
)

catkin_package(
   INCLUDE_DIRS include
   CATKIN_DEPENDS
      roscpp
      sensor_msgs
      nav_msgs
      geometry_msgs
      std_msgs
      gazebo_msgs
)

include_directories(
  include
  ${catkin_INCLUDE_DIRS}
)

add_executable(
   ${PROJECT_NAME}
      src/pid_control_node.cpp
      src/BotControl.cpp
)

target_link_libraries(${PROJECT_NAME}
   ${catkin_LIBRARIES}
)
