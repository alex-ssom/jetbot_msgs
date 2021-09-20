cmake_minimum_required(VERSION 3.0.2)
project(jetbot_msgs)

find_package(catkin REQUIRED COMPONENTS
    message_generation
)

## Generate messages in the 'msg' folder
add_message_files(
  FILES
  motors_raw.msg
)

## Generate services in the 'srv' folder
# add_service_files(
#   FILES
#   Service1.srv
#   Service2.srv
# )

generate_messages(
    DEPENDENCIES
)

catkin_package(
    CATKIN_DEPENDS message_runtime
)
