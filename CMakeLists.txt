cmake_minimum_required(VERSION 3.0.2)
project(aidi_axio_description)

add_compile_options(-std=c++14)

find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY
    mesh
    urdf
    config
    launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
