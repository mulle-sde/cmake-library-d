cmake_minimum_required(VERSION 3.10)
project(d VERSION 0.1.0)

add_library(d SHARED src/d.c)
target_include_directories(d PUBLIC include)

install(TARGETS d)
install(FILES include/d/d.h DESTINATION include/d)
