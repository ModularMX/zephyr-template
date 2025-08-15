# Minimum CMake required version
cmake_minimum_required( VERSION 3.20.0 )

# set enviroemnt variables like the board nad the debug server
#set(BOARD nrf54l15dk/nrf54l15/cpuapp)
set(BOARD_FLASH_RUNNER jlink)

# Get Zephyr directory
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

# Project and source files
project(template)
target_sources(app PRIVATE src/main.c)