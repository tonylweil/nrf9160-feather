#
# Copyright (c) 2019 Nordic Semiconductor ASA
#
# SPDX-License-Identifier: Apache-2.0
#

cmake_minimum_required(VERSION 3.13.1)
find_package(Zephyr HINTS $ENV{ZEPHYR_BASE})
project(dht22)

FILE(GLOB app_sources src/*.c)
target_sources(app PRIVATE ${app_sources})
