cmake_minimum_required(VERSION 3.16.x)
project(mongoDB-test)

# Specify the minimum version you require.
find_package (mongoc-1.0 1.7 REQUIRED)

# The "hello_mongoc.c" sample program is shared among four tests.
add_executable (main ../main.c)
target_link_libraries (main PRIVATE mongo::mongoc_shared)