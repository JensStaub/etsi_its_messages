cmake_minimum_required(VERSION 3.5)
project(etsi_its_mcm_msgs)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

set(msg_files
  "msg/AdvisedTrrContainer.msg"
  "msg/Altitude.msg"
  "msg/AltitudeConfidence.msg"
  "msg/AltitudePosition.msg"
  "msg/AltitudeValue.msg"
  "msg/CurrentStateAdvisedChange.msg"
  "msg/GenerationDeltaTime.msg"
  "msg/HeadingValue.msg"
  "msg/Identifier1B.msg"
  "msg/Iso3833VehicleType.msg"
  "msg/ItsPduHeader.msg"
  "msg/JoinGroupStateChange.msg"
  "msg/KinematicsCharacteristics.msg"
  "msg/LaneCount.msg"
  "msg/Latitude.msg"
  "msg/LatitudePosition.msg"
  "msg/ListOfSubmanoeuvreDescriptionsContainer.msg"
  "msg/Longitude.msg"
  "msg/LongitudePosition.msg"
  "msg/MCM.msg"
  "msg/ManoeuvreAdvice.msg"
  "msg/ManoeuvreAdviceContainer.msg"
  "msg/ManoeuvreCooperationCost.msg"
  "msg/ManoeuvreCooperationGoal.msg"
  "msg/ManoeuvreCoordinationConcept.msg"
  "msg/ManoeuvreCoordinationRational.msg"
  "msg/ManoeuvreExecutionStatus.msg"
  "msg/ManoeuvreId.msg"
  "msg/ManoeuvreOverallStrategy.msg"
  "msg/McmBasicContainer.msg"
  "msg/McmContainer.msg"
  "msg/McmGenericCurentStateContainer.msg"
  "msg/McmItssRole.msg"
  "msg/McmStationType.msg"
  "msg/McmType.msg"
  "msg/MessageId.msg"
  "msg/OrdinalNumber1B.msg"
  "msg/PosConfidenceEllipse.msg"
  "msg/ReferencePosition.msg"
  "msg/SemiAxisLength.msg"
  "msg/SpecialTransportType.msg"
  "msg/Speed.msg"
  "msg/SpeedConfidence.msg"
  "msg/SpeedValue.msg"
  "msg/StationId.msg"
  "msg/Submanoeuvre.msg"
  "msg/SubmanoeuvreDescription.msg"
  "msg/SubmanoeuvreStrategy.msg"
  "msg/Submanoeuvres.msg"
  "msg/TRRLength.msg"
  "msg/TRRWidth.msg"
  "msg/TemporalCharacteristics.msg"
  "msg/Trajectory.msg"
  "msg/TrrDescription.msg"
  "msg/TrrType.msg"
  "msg/VehicleCurrentStateContainer.msg"
  "msg/VehicleHeight.msg"
  "msg/VehicleLength.msg"
  "msg/VehicleLengthConfidenceIndication.msg"
  "msg/VehicleLengthValue.msg"
  "msg/VehicleManoeuvreContainer.msg"
  "msg/VehicleSize.msg"
  "msg/VehicleWidth.msg"
  "msg/WayPoint.msg"
  "msg/WayPointType.msg"
  "msg/Wgs84Angle.msg"
  "msg/Wgs84AngleConfidence.msg"
  "msg/Wgs84AngleValue.msg"
)

rosidl_generate_interfaces(${PROJECT_NAME}
  ${msg_files}
)

ament_export_dependencies(rosidl_default_runtime)

ament_package()
