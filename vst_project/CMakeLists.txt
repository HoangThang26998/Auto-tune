cmake_minimum_required(VERSION 3.15)

project(HT_Audio_98_Suite VERSION 1.0.0 LANGUAGES CXX)

set(JUCE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/JUCE CACHE PATH "Path to JUCE")
add_subdirectory(AutoKey)
add_subdirectory(AutoTune11)
