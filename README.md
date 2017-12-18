# mingw_w64-qt5_static-cmake-console-example
A "Hello, world" console application using statically compiled Qt 5 by MinGW-w64 in 64 bit and CMake

# How to build
 - download https://github.com/tim-lebedkov/packages/releases/download/initial/com.nokia.QtDev-x86_64-w64-Npackd-Release-5.5.7z and unpack it into C:\NpackdSymlinks\com.nokia.QtDev-x86_64-w64-Npackd-Release-5.5
 - download CMake from https://www.cmake.org/files/v3.10/cmake-3.10.1-win32-x86.zip and unpack it into "C:\Program Files\CMake"
 - download MinGW-w64 from https://github.com/tim-lebedkov/packages/releases/download/2016_Q1/x86_64-4.9.2-release-posix-seh-rt_v3-rev1.7z and unpack it into C:\Program Files\MinGW-w64_x86_64_SEH_POSIX_threads
 - open console and change to the directory with this README.md
 - mkdir build
 - cd build
 - set PATH=C:\Program Files\CMake\bin;C:\Program Files\MinGW-w64_x86_64_SEH_POSIX_threads\bin;%path%
 - cmake ..\ -G "MinGW Makefiles"
 - mingw32-make
 - qt_5_cmake_console.exe