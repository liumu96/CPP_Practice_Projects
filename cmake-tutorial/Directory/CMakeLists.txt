cmake_minimum_required(VERSION 3.21)

project(directory_test)

# Bring the headers, such as Student.h into the project
include_directories(include)

# Can manually add the source using the set command as follows:
# set(SOURCES src/mainapp.cpp src/Student.cpp)

# However, this file(GLOB...) allows for wildcard additions:
file(GLOB SOURCES "src/*.cpp")

add_executable(directory_test ${SOURCES})

