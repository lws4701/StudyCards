cmake_minimum_required(VERSION 3.27)
project(StudyCards)

set(CMAKE_CXX_STANDARD 11)
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/deps/SQLiteCpp-3.3.1)
add_executable(StudyCards main.cpp)
target_link_libraries(StudyCards
        SQLiteCpp
        sqlite3
        )