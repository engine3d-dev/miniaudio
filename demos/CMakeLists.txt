cmake_minimum_required(VERSION 3.27)
project(demos CXX)

build_application(
    SOURCES
    application.cpp

    PACKAGES
    miniaudio

    LINK_PACKAGES
    miniaudio::miniaudio
)