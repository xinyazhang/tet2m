# tet2m
Another simple tool, which converts tetgen output files to Wolfram Language.

## Build
To build

    mkdir build
    cd build
    cmake ..
    make

## Install

Copy tet2m to anywhere you like.
No `make install` target is provided since this is really a tiny tool.

## Use
```tet2m -i <prefix of tetgen files> [-o output_file]```

Since this tool takes .node and .ele as input files, for simplicity the common
prefix is asked, rather than the node and ele files.

For example, ```tet2m -i tet -o test.m``` will read `tet.node` and `tet.ele` and
write the data to `test.m`.

## Limitations

1. No support for attributes in .node or .ele files.
2. No support for discontinuous vertex indices in .node file
