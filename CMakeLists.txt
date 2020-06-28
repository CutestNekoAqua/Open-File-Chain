cmake_minimum_required(VERSION 3.10)

# set the project name and version
project(OpenFileChain VERSION 1.0)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(OpenFileChain src/main.cpp src/Block.cpp src/Blockchain.cpp)
include_directories("src" "lib" "include")
target_include_directories(OpenFileChain PUBLIC "src" "lib" "include")
install(TARGETS OpenFileChain DESTINATION bin)
