cmake_minimum_required(VERSION 3.11.3)

set(CMAKE_CXX_STANDARD 17)

project(Membot)

#find_package(wxWidgets CONFIG REQUIRED)
set(CMAKE_PREFIX_PATH  C:/wxWidgets-3.2.4) 
#find_package(wxWidgets REQUIRED COMPONENTS core base)
file(GLOB project_SRCS src/*.cpp)

#include(${wxWidgets_USE_FILE})

add_executable(membot ${project_SRCS})
target_link_libraries(membot ${wxWidgets_LIBRARIES})
#target_link_libraries(membot PRIVATE wx::core wx::base)



set(CMAKE_PREFIX_PATH  C:/dev/wxWidgets/lib/cmake/wxWidgets)

