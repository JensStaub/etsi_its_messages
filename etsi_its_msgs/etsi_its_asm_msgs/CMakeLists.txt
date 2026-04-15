cmake_minimum_required(VERSION 3.5)
project(etsi_its_asm_msgs)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

set(msg_files
  "msg/ASM.msg"
  "msg/ApplicationIdentifier.msg"
  "msg/ApplicationSpecificData.msg"
  "msg/ApplicationSpecificMessage.msg"
  "msg/ItsPduHeader.msg"
  "msg/StationID.msg"
  "msg/TimestampIts.msg"
)

rosidl_generate_interfaces(${PROJECT_NAME}
  ${msg_files}
)

ament_export_dependencies(rosidl_default_runtime)

ament_package()
