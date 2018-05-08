
cmake_minimum_required(VERSION 3.10)
 
PROJECT(NESRINE)

find_package( Qt5Core REQUIRED )

find_package(VTK REQUIRED)
include(${VTK_USE_FILE})

file( GLOB nesrine_SRC
	"source/main.cpp"
)
add_executable(NESRINE ${nesrine_SRC} )
 
target_link_libraries(NESRINE ${VTK_LIBRARIES} Qt5::WinMain)
