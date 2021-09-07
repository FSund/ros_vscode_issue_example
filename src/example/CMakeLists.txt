cmake_minimum_required(VERSION 3.0.2)
project(example)

find_package(catkin REQUIRED)

catkin_python_setup()

catkin_package()

include_directories()

catkin_install_python(PROGRAMS
  src/executable.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
