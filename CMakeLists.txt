cmake_minimum_required (VERSION 3.1.10)

project(robot_control_learning)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

aux_source_directory (src SRC_LIST)

include_directories(include)

add_executable(main ${SRC_LIST})

