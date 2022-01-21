cmake_minimum_required(VERSION 3.0.0)
project(ChatServerClient VERSION 0.1.0)

add_subdirectory(ChatServer)
add_subdirectory(ChatClient)

include(CTest)
enable_testing()
set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
