# CMakeList.txt: проект CMake для second_CMake; включите исходный код и определения,
# укажите здесь логику для конкретного проекта.
#

# Добавьте источник в исполняемый файл этого проекта.
add_executable (second_CMake "second_CMake.cpp" "second_CMake.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET second_CMake PROPERTY CXX_STANDARD 20)
endif()

# TODO: Добавьте тесты и целевые объекты, если это необходимо.
