## Overview
This project appears to be a simple 3D model viewer for a robotic arm. It allows the user to rotate and manipulate the joints of a robotic arm by adjusting their angles through integer arrays. The project is built using C programming language and makes use of various libraries for graphics rendering, input handling, and data structure management.

## Features
- **Robotic Arm Model**: The model consists of multiple bones with joints that can be manipulated.
- **Joint Manipulation**: Users can adjust the angles of the robotic arm's joints by providing integer arrays representing the path to each joint and the desired angle value.
- **Rendering**: The robotic arm is rendered in a 3D space, allowing users to visualize the current state of the arm.

## Project Structure
The project structure is well-organized, with different files and directories serving specific purposes:
- `src/`: Contains the source code for the project. It includes `Main.c` which serves as the entry point, and various header files `.h`.
- `Makefile.linux`, `Makefile.windows`, `Makefile.wine`, `Makefile.web`: These are build configuration files tailored for different platforms.
- `README.md`: This document describes the project.

### Prerequisites
To build and run this project, you will need:
- A C/C++ Compiler (GCC/Clang)
- Make utility
- Standard development tools

## Build & Run
The build process involves using Makefiles specific to each platform. Below are the steps for building the project on different operating systems:

### Linux
To build the project on a Linux system, follow these steps:
```bash
cd <Project>
make -f Makefile.linux all
```
This will compile the source code and generate executable files in the `build/` directory.

### Windows
For Windows, use the following command:
```bash
cd <Project>
make -f Makefile.windows all
```

### Wine (Cross-Compile for Windows on Linux)
To build the project on Linux but produce a Windows executable:
```bash
cd <Project>
make -f Makefile.wine all
```

### Emscripten (WebAssembly)
For building the project into WebAssembly:
```bash
cd <Project>
make -f Makefile.web all
```

## Build Options
- `make -f Makefile.(os) all`: Builds the output executable.
- `make -f Makefile.(os) do`: Builds and runs the executable.
- `make -f Makefile.(os) clean`: Removes build artifacts.

### Execute
Once built, you can run the project using:
```bash
make -f Makefile.(os) exe
```

This README provides a comprehensive overview of the project structure, features, prerequisites, and build instructions.