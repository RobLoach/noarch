cmake_minimum_required(VERSION 3.0)
project(noarch
	VERSION 1.2.0
	LANGUAGES C )

add_executable(noarch noarch.c)
target_compile_options(noarch PRIVATE -Wall -Wextra -pedantic -Werror)
target_link_libraries(noarch dl)
