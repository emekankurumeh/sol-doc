$title=Building Sol

## Requirements

$raw$

+ `gcc` or `clang` is used to compile
+ `SDL1.2` is linked to dynamically
+ `LuaJIT` is linked to dynamically, although this is optional as non-JIT Lua can be used in its place
+ `Python2.7` is used by the build script

$/raw$


These dependencies must be met before building.

## Building
Sol can be built on Linux, Windows and OS X. To build you should first clone the repo and cd into it

$raw$

    git clone https://github.com/emekankurumeh/sol.git
    cd sol

$/raw$


The build script should then be executed:

$raw$

    ./build.py

$/raw$


On windows:

$raw$

    python build.py

$/raw$


When the build is finished an executable named `sol` (or `sol.exe` on windows) should exist in the `bin/` directory.

You can test it works by executing one of the example projects:


$raw$

    ./bin/sol example/particles

$/raw$


On windows:

$raw$

    bin/sol example/particles

$/raw$


## Build options
The following arguments can be passed to the `build.py` script:

$raw$

+ `debug` - compiles unoptimized and doesn't strip debug symbols
+ `nojit` - uses embedded Lua instead of linking to LuaJIT

$/raw$
