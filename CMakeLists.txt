cmake_minimum_required(VERSION 2.6)
project(test_cplus)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -g  ")
set(SRC_FILE enum_union.cpp
	operator/operate.cpp
	smart_pointer/my_allocator.cpp
)
add_executable(test_cplus main.cpp ./funcation/funcation.cpp ./stream/my_fstream.cpp ./friend/my_friend.cpp ${SRC_FILE})


add_subdirectory(template)
add_subdirectory(throw_try_catch)
add_subdirectory(friend)
add_subdirectory(boost)
add_subdirectory(algorithm)
add_subdirectory(oop)
# add_subdirectory(move)
# add_subdirectory(common)
add_subdirectory(design_pattern)
