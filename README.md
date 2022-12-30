This fork of [zlib](https://zlib.net) provides a script to amalgamate the
source code into a single `zlib_amalgamated.c` and `zlib_amalgamated.h`.

A small number of patches are applied, which you can find by searching the
`git log` for commits made by `Ayman El Didi`.

## Usage

Go to the [releases](https://github.com/aeldidi/zlib/releases) page and
download the latest release, which contains a self contained `zlib.c` and
`zlib.h` which you can simply compile and use.

## To Amalgamate It Yourself

Compile `tools/amalgamate.c` into a an executable and run it like so:

```
$ amalgamate <path to repository root>
```

This will generate `zlib_amalgamated.c` and `zlib_amalgamated.h` in the
directory it was run from.
