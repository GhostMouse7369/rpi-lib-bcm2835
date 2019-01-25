cmake_minimum_required(VERSION 3.13)
project(bcm2835 C)

set(CMAKE_C_STANDARD 99)

SET(LIBRARY_OUTPUT_PATH ./libs)

aux_source_directory(./src DIR_SRCS)

add_library(bcm2835 SHARED ${DIR_SRCS})