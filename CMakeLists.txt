cmake_minimum_required(VERSION 3.16.0)
include($ENV{IDF_PATH}/tools/cmake/project.cmake)
project(pio-lvgl_esp32-reproduce)

get_filename_component(configName "${CMAKE_BINARY_DIR}" NAME)
list(APPEND kconfigs "${CMAKE_SOURCE_DIR}/.pio/libdeps/${configName}/lvgl_esp32_drivers/Kconfig")
list(APPEND kconfigs "${CMAKE_SOURCE_DIR}/.pio/libdeps/${configName}/lvgl/Kconfig")
