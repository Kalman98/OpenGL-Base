cmake_minimum_required( VERSION 2.8 )

project( OpenGL )

include_directories( include/ )
add_executable( main main.cpp glad.c )
target_link_libraries( main ${CMAKE_SOURCE_DIR}/lib/libglfw3.a GL X11 pthread Xrandr Xi dl Xxf86vm Xinerama Xcursor)
