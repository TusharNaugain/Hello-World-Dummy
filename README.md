HelloWorldProject

A simple C++ "Hello, World!" project built using CMake.

Project Structure
css
Copy code
HelloWorldProject/
├── CMakeLists.txt
└── src/
    └── main.cpp
Prerequisites
CMake version 3.10 or higher
C++ Compiler (e.g., g++, clang++)


Getting Started
Follow these instructions to set up, build, and run the project.

Step 1: Clone the Repository
If this project is in a repository, clone it. Otherwise, navigate to the project directory.
git clone https://github.com/TusharNaugain/Hello-World-Dummy.git
cd HelloWorldProject.


Step 2: Write the Code
Make sure your src/main.cpp file contains the following code:
#include <iostream>
int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}


Step 3: Configure CMake
Create a file named CMakeLists.txt in the root directory with the following content:
cmake
cmake_minimum_required(VERSION 3.10)
project(HelloWorldProject VERSION 1.0)
add_executable(hello_world src/main.cpp)

Step 4: Create a Build Directory
Create and navigate to a build directory for compiling the project.
mkdir build
cd build

Step 5: Build the Project
Use CMake to configure the project and generate build files, then compile it with make.
cmake ..
make

Step 6: Run the Program
After building, execute the compiled program:
./hello_world
Expected output:
Hello, World!


Troubleshooting
Ensure Correct File Paths: Verify that main.cpp is located in the src folder and CMakeLists.txt has the correct path to it.
Clean Build Directory: If errors persist, remove all contents of the build directory and repeat the build steps.


License
This project is licensed under the MIT License.
