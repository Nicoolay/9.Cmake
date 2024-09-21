
cmake_minimum_required (VERSION 3.8)

if (POLICY CMP0141)
  cmake_policy(SET CMP0141 NEW)
  set(CMAKE_MSVC_DEBUG_INFORMATION_FORMAT "$<IF:$<AND:$<C_COMPILER_ID:MSVC>,$<CXX_COMPILER_ID:MSVC>>,$<$<CONFIG:Debug,RelWithDebInfo>:EditAndContinue>,$<$<CONFIG:Debug,RelWithDebInfo>:ProgramDatabase>>")
endif()
include_directories(${CMAKE_SOURCE_DIR}/Figures)


add_executable (second_CMake second_CMake/second_CMake.cpp 
second_CMake/Equilateral_triangle.cpp 
second_CMake/Equilateral_triangle.h 
second_CMake/Figure.cpp 
second_CMake/Figure.h 
second_CMake/Isosceles_triangle.cpp 
second_CMake/Isosceles_triangle.h 
second_CMake/Parallelogram.cpp 
second_CMake/Parallelogram.h 
second_CMake/Quadrangle.cpp 
second_CMake/Quadrangle.h 
second_CMake/Rect.cpp 
second_CMake/Rect.h 
second_CMake/Rhombus.cpp 
second_CMake/Rhombus.h 
second_CMake/Right_triangle.cpp 
second_CMake/Right_triangle.h
second_CMake/Square.cpp 
second_CMake/Square.h 
second_CMake/Triangle.cpp 
second_CMake/Triangle.h)
