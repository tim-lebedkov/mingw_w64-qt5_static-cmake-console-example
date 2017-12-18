cmake_minimum_required(VERSION 2.8.12)
project(qt-5-cmake-console)

set(qt_location "C:\\NpackdSymlinks\\com.nokia.QtDev-x86_64-w64-Npackd-Release-5.5")

LIST(APPEND CMAKE_PREFIX_PATH "${qt_location}\\qtbase\\lib\\cmake\\Qt5Core") 

# Tell CMake to run moc when necessary:
set(CMAKE_AUTOMOC ON)

# As moc files are generated in the binary dir, tell CMake
# to always look for includes there:
set(CMAKE_INCLUDE_CURRENT_DIR ON)

link_directories("${qt_location}\\qtbase\\lib") 

find_package(Qt5Core REQUIRED)

add_executable(qt_5_cmake_console "src/main.cpp")

target_link_libraries(qt_5_cmake_console Qt5::WinMain Qt5::Core qtpcre ws2_32)


