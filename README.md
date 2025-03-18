# GNU C-Compiler for ARM

The GNU C-Compiler for ARM in a Debian image.

See [Docker-Hub](https://hub.docker.com/r/st3ph4n/gcc-arm-none-eabi/)

See [Github](https://github.com/rstephan/docker-gcc-arm-none-eabi)


## Usage

To use the image call something like this:

```
$ docker run --rm -v $(pwd):/build st3ph4n/gcc-arm-none-eabi make
```

This puts your current work directory into the container, builds your code and
afterwards it removes the container.

You can use `make`, `cmake` or call the gcc directly.

## Example output

```
$ docker run --rm st3ph4n/gcc-arm-none-eabi arm-none-eabi-gcc --version
arm-none-eabi-gcc (15:12.2.rel1-1) 12.2.1 20221205
Copyright (C) 2022 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```
