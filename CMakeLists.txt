project(HelloWorld)
cmake_minimum_required(VERSION 3.0)

add_executable(hello-world main.cpp)

# enable testing functionality
enable_testing()
add_test(NAME hello-world-TEST, COMMAND hello-world)

install(TARGETS hello-world RUNTIME DESTINATION bin)
include(CPack)
