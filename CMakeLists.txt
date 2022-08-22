cmake_minimum_required(VERSION 3.16)
project(imgui CXX)

include_directories(
        "."
)

add_library(${PROJECT_NAME} STATIC "")
target_sources(${PROJECT_NAME} PRIVATE
        "imconfig.h"
        "imgui.cpp"
        "imgui.h"
        "imgui_demo.cpp"
        "imgui_draw.cpp"
        "imgui_internal.h"
        "imgui_tables.cpp"
        "imgui_widgets.cpp"
        "imstb_rectpack.h"
        "imstb_textedit.h"
        "imstb_truetype.h"
        )
target_include_directories(${PROJECT_NAME} PUBLIC
        "."
)
