cmake_minimum_required(VERSION 2.8.3)
project(rosbag_tools)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  cv_bridge
  image_transport
)

catkin_package(
  INCLUDE_DIRS include
#  LIBRARIES rosbag_tools
  CATKIN_DEPENDS roscpp rospy std_msgs
  DEPENDS system_lib
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

add_executable(
	image_converter 
	src/image_converter.cpp
)

target_link_libraries(
	image_converter
	${catkin_LIBRARIES}
)
