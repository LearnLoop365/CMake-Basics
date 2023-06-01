# CMake to Generate `makefile` to Print Hello World


## `CMakeLists.txt`
```
add_custom_target(foo ALL)

add_custom_command(
	TARGET foo
	COMMAND echo Hello World
)
```


## `cmake` Command
```
cmake -G "Unix Makefiles" -Wno-dev -D CMAKE_TARGET_MESSAGES=off -B build .
```

`-Wno-dev` for Suppressing Warning about Missing `project()`
`-D CMAKE_TARGET_MESSAGES=off` for Disabling Report the Completion of Each Target
`.` for the Source Tree
`-B build` for the Build Tree


## `make` Command
```
cd build
make
```
