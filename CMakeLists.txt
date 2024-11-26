cmake_minimum_required(VERSION 3.28)
project(ImGuiOpenGL-Example)

set(CMAKE_CXX_STANDARD 20)

add_executable(ImGuiOpenGL-Example main.cpp
        imgui/imconfig.h
        imgui/imgui.cpp
        imgui/imgui.h
        imgui/imgui_demo.cpp
        imgui/imgui_draw.cpp
        imgui/imgui_impl_opengl3.cpp
        imgui/imgui_impl_opengl3.h
        imgui/imgui_impl_opengl3_loader.h
        imgui/imgui_impl_win32.cpp
        imgui/imgui_impl_win32.h
        imgui/imgui_internal.h
        imgui/imgui_tables.cpp
        imgui/imgui_widgets.cpp
        imgui/imstb_rectpack.h
        imgui/imstb_truetype.h
        imgui/imstb_textedit.h
)

target_link_libraries(ImGuiOpenGL-Example PRIVATE
        winmm
        opengl32
)