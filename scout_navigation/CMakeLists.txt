cmake_minimum_required(VERSION 3.10.2)
project(scout_navigation)

find_package(catkin REQUIRED roslaunch)

catkin_package()

roslaunch_add_file_check(launch)

install(
  DIRECTORY config launch maps rviz
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

