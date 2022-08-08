cmake_minimum_required(VERSION 3.22)

project(imgui)

add_library(imgui imconfig.h imgui.h imgui.cpp imgui_draw.cpp imgui_internal.h imgui_tables.cpp imgui_widgets.cpp imstb_rectpack.h imstb_textedit.h imstb_truetype.h imgui_demo.cpp)
target_include_directories(imgui PUBLIC imgui.h imconfig.h imgui_internal.h imstb_rectpack.h imstb_textedit.h imstb_truetype.h backends/)