cmake_minimum_required(VERSION 3.10)
project(game-4096)

set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(SRC
   "src/main.c"
)

add_executable(game-4096 ${SRC})
target_compile_options(game-4096 PRIVATE -Wall -Wextra -Wpedantic -O0 -g)
