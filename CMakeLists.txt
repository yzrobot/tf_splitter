cmake_minimum_required (VERSION 2.8.3)
project(tf_splitter)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  tf
  )

###################################
## catkin specific configuration ##
###################################

catkin_package()

###########
## Build ##
###########

include_directories(include
  ${catkin_INCLUDE_DIRS}
  )

add_executable(${PROJECT_NAME}
  src/tf_splitter.cpp
  )

target_link_libraries(${PROJECT_NAME}
  ${catkin_LIBRARIES}
  )

#############
## Install ##
#############

install(TARGETS ${PROJECT_NAME}
  RUNTIME DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
  )
