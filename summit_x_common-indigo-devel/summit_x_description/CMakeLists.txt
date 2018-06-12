cmake_minimum_required(VERSION 2.8.3)
project(summit_x_description)

find_package(catkin REQUIRED robot_state_publisher urdf xacro robotnik_sensors)

catkin_package(
  CATKIN_DEPENDS urdf xacro
)

install(
  DIRECTORY launch meshes urdf robots config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
