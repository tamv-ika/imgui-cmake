cmake_minimum_required(VERSION 3.13)

project(imgui)

add_library(
    imgui
    STATIC
    ${CMAKE_CURRENT_SOURCE_DIR}/imgui/imgui.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/imgui/imgui_demo.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/imgui/imgui_draw.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/imgui/imgui_tables.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/imgui/imgui_widgets.cpp
)

target_include_directories( imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/imgui)
set_target_properties( imgui PROPERTIES FOLDER "imgui")