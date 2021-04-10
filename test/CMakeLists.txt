set(NAME ce-config-test)
file(GLOB_RECURSE SRC
	"*.hpp"
	"*.cpp"
	"*.c"
)

add_executable(${NAME}
#WIN32
${SRC}
)



target_link_libraries(${NAME}
	ce-config
)

include_directories(${NAME}
	"${CMAKE_SOURCE_DIR}/src/"
)
