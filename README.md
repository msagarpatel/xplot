# xplot for macOS

This project takes the most recent version of xplot (v0.90.7.1 from Sept. 19,
2003!), and ports it forward so xplot may be built on macOS. The original source
of xplot was taken from [xplot.org](http://xplot.org). Only the most minimal
changes required to build, install, run, and uninstall xplot on macOS have been
made. No substantial features have been added, nor are any features planned.

xplot's README is [README](README).


## Dependencies
X11 is required, and can be installed via:
- [Homebrew](https://brew.sh) with `brew install xquartz`, or
- direct download from [xquartz.org](https://www.xquartz.org).


## Installation
Simply run
```shell
./configure
make
make install
```
to build and install xplot. Then, run xplot like so
```shell
xplot /path/to/xplot/file
```
The following man pages are also installed: `xplot(1)` and `tcpdump2xplot(1)`.


## Support
This project has been tested on macOS Big Sur 11.2. I'd love to hear if you
successfully build and run this project on another system. Please open an issue
to let me know.


## Uninstallation
If xplot was installed with `make install`, then it may be uninstalled using
```shell
make uninstall
```


## Contributing
Pull requests that add support or documentation for more operating systems are
welcome.
