# Graphics Lab - OpenGL Cyan Star

## Student Information
* **Name:** Hasib Al Mahmud Siddique
* **ID:** 095

## Project Description
This project is a simple 2D computer graphics application built using C++ and modern OpenGL (Core Profile). It renders a cyan-colored, 5-pointed star centered on a yellow background. 

As per the assignment requirements, the star is geometrically constructed using exactly 5 intersecting triangles (15 vertices) rather than a continuous polygon outline or complex shader math.

## Features
* **Custom Geometry:** Renders a perfect star using a 5-triangle overlapping technique.
* **Custom Colors:** Utilizes Fragment Shaders to output a solid Cyan star (`vec4(0.0, 1.0, 1.0, 1.0)`) against a `glClearColor` Yellow background (`1.0, 1.0, 0.0, 1.0`).
* **Custom Window Property:** The window title is set to the student ID ("095").
* **Custom Input Handling:** The application listens for the initial letter of the student's name. Pressing the **'H'** key will safely close the window and terminate the program.

## Prerequisites
To build and run this project, the following tools are required:
* **Compiler:** 32-bit MinGW GCC (e.g., `mingw-w64-i686-gcc` via MSYS2)
* **Build Tool:** GNU Make (`make`)
* **Libraries:** * GLFW 3.4 (32-bit Windows Binaries)
  * GLAD (OpenGL loader)

## Project Structure
* `src/main.cpp` - The main application logic, render loop, and shader definitions.
* `src/glad.c` - The GLAD loader source file.
* `include/` - Contains the required `glad.h`, `glfw3.h`, and `khrplatform.h` header files.
* `lib/` - Contains the static library `libglfw3.a` and dynamic library `glfw3.dll`.
* `Makefile` - Contains the build instructions.

## Build Instructions
1. Open a terminal (VS Code Terminal or Command Prompt) and navigate to the project root folder.
2. Run the following command to compile the project:
   ```bash
   make win
