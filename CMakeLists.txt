cmake_minimum_required(VERSION 3.16.0)

list (APPEND EXTRA_COMPONENT_DIRS "${CMAKE_CURRENT_LIST_DIR}/components/esp-aws-iot/libraries/"
    )

include($ENV{IDF_PATH}/tools/cmake/project.cmake)
include_directories(BEFORE "${CMAKE_CURRENT_LIST_DIR}/src")
project(tngtest-awsiot-mqttagent)
