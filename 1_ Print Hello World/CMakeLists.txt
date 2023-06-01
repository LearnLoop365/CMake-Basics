add_custom_target(foo ALL)

add_custom_command(
	TARGET foo
	COMMAND echo Hello World
)