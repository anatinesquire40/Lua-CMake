# Lua Project Setup

## Description

This repository contains a custom build of Lua, including the interpreter (`lua`), the Lua compiler (`luac`), and the shared Lua library (`lua54`). The build system uses CMake, and it simplifies the process of compiling for multiple platforms such as Windows, Linux, and Android.

### Components:
- **lua54**: Shared Lua library.
- **lua**: The Lua interpreter.
- **luac**: The Lua compiler (bytecode compiler).
- **wlua**: Windows-specific Lua, only for Windows environments.

Each component has its own `CMakeLists.txt` file to manage the build process.

### Build Process:
1. **Clone the Repository**
   
   Clone this repository into the following directory path:
   ```plaintext
   lua-src(from lua.org)/src
   ```

2. **Building the Project**

    Inside the project, you’ll find a directory called `build-all`. This folder contains the necessary build files for all components, so you can build them without needing to run the build process separately for each one.

3. **Platform Specifics**

    - **wlua** is only required for **Windows**.
    - **lua54** (shared library), **lua** (interpreter), and **luac** (compiler) can be built for **Linux** and **Android** as well.

4. **Build Process**

    After cloning the repository, navigate to the `build-all` folder and run the CMake build process to compile everything.

---

### Credits

- **Lua.org**: The Lua source code is from [Lua.org](https://lua.org), the original creators and maintainers of the Lua programming language.
- **CMake**: The build system used for managing the compilation process is powered by [CMake](https://cmake.org).
- **Developer**: Special thanks to **AnatineSquire40** for the custom build and modifications of Lua for various platforms.

Thank you for using this project! If you encounter any issues or have questions, feel free to reach out.