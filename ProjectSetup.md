# Project setup

## C/C++ Setup
![Language](https://img.shields.io/badge/language-C/C++-brightgreen)
![CMake](https://img.shields.io/badge/build-CMake-blue)
1. Ensure you have the following VS Code extensions installed:
- [C/C++ Extension Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-extension-pack)
- [CMake Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools)
2. Create the following in your main directory:
- Directory `include` for your header (`.h/.hpp`) files.
- Directory `src` for your implementation (`.c/.cpp`) files.
- Create a `main.c`/`main.cpp` file in the `src` directory with your main function.
- File `CMakeLists.txt`
3. Copy this template into your `CMakeListsFile.txt` file:
```cmake
cmake_minimum_required(VERSION 3.16)
project(<project name>)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)

file(GLOB_RECURSE SOURCES "src/*.c" "src/*.cpp")
add_executable(<executable file name> ${SOURCES})

include_directories(include)
```
Replace `<project name>` and `<executable file name>` with your desired names.

4. Press `F1` and type the following, followed by an enter: `Cmake: Configure`
5. Select the compiler you want to use.
6. Press `F1` and type the following, followed by an enter: `Cmake: Build`
7. Use the `⚙️Build` button to build your project, the `🪲` button to debug your project, and the `▶️` button to run your project, located in the status bar at the bottom left.
