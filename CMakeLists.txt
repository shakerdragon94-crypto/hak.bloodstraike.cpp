cmake_minimum_required(VERSION 3.10.2)
project(bloodstrike_mod)

add_library(
    bloodstrike_mod
    SHARED
    bloodstrike_jni.cpp
)

find_library(
    log-lib
    log
)

target_link_libraries(
    bloodstrike_mod
    ${log-lib}
)
