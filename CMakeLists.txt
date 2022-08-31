cmake_minimum_required(VERSION 3.22)

project(imgui)

add_library(imgui imconfig.h imgui.h imgui.cpp imgui_draw.cpp imgui_internal.h imgui_tables.cpp imgui_widgets.cpp imstb_rectpack.h imstb_textedit.h imstb_truetype.h imgui_demo.cpp)
target_include_directories(imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

target_compile_definitions(imgui PUBLIC IMGUI_IMPL_OPENGL_LOADER_CUSTOM)

set(CMAKE_CXX_FLAGS "-fPIC")
