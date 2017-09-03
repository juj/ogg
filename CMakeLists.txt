cmake_minimum_required(VERSION 2.8)

project(ogg)

#add_definitions(-Wall -Wcast-qual -Wextra -Wshadow -fno-exceptions -fno-rtti -pedantic -flto -m64)

include_directories(include)

file(GLOB_RECURSE sourceFiles src/*.c)
file(GLOB_RECURSE headerFiles include/*.h)

add_library(ogg STATIC ${sourceFiles} ${headerFiles})
