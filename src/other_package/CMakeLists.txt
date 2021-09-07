cmake_minimum_required(VERSION 3.0.2)
project(other_package)

find_package(catkin REQUIRED example)

catkin_package()

include_directories()

catkin_install_python(PROGRAMS
  src/executable.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
