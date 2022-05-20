cmake_minimum_required(VERSION 3.21)
project(simulare)

set(CMAKE_CXX_STANDARD 14)

add_executable(simulare main.cpp Gui.cpp Gui.h Candidat.cpp Candidat.h Repo.cpp Repo.h Tests.cpp Tests.h Service.cpp Service.h)

set(CMAKE_PREFIX_PATH "C:\\Qt\\6.2.4\\mingw_64\\lib\\cmake")
find_package(Qt6Widgets REQUIRED)
target_link_libraries(simulare Qt6::Widgets)
