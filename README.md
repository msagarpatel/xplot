# xplot for macOS

This project takes the most recent version of xplot (v0.90.7.1 from Sept. 19,
2003!), and ports it forward so xplot may be built on macOS. The original source
of xplot was taken from [xplot.org](http://xplot.org). Only the most minimal
changes required to build and run xplot on macOS have been made. No substantial
features have been added, nor are any features planned.

xplot's README is [README](README).


## Dependencies
X11 is required, and can be installed via:
- [Homebrew](https://brew.sh) with `brew install xquartz`, or
- direct download from [xquartz.org](https://www.xquartz.org).


## Installation
Simply run
```shell
./configure && make
```
to build xplot. Then, run xplot like so
```shell
./xplot /path/to/xplot/file
```
This has been tested on macOS 11.2 and Ubuntu 16.04. I'd love to hear if you
successfully build and run this project on another system. Please open an issue
to let me know.


## Contributing
Pull requests that add support or documentation for more operating systems are
welcome.
