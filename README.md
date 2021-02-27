# xplot for macOS

This project takes the most recent version of xplot (v0.90.7.1 from Sept. 19,
2003!), and ports it forward so xplot may be built on macOS. The original source
of xplot was taken from [xplot.org](http://xplot.org).

xplot's README is [README](README).


## Dependencies
X11 is required, and can be installed via:
- [Homebrew](https://brew.sh) with `brew install xquartz`, or
- direct download from [xquartz.org](https://www.xquartz.org).

Either method should have installed X11 at `/opt/X11`. If not, create a symbolic
link to that path, or modify the paths in the parameters to `./configure`
described [below](#macOS).


## Installation
### macOS
At the moment, the configure script is unable to automatically detect whether
X11 is installed, so we manually provide it's location. So, xplot is built by
running:
```shell
./configure --x-includes=/opt/X11/include --x-libraries=/opt/X11/lib
make
```

### All other operating systems
If `./configure && make` do not suffice, run `git clean -xf`, and then try the
instructions for [macOS above](#macOS). If you compiled xplot on another system,
I'd love to hear how you did it. Please open an issue to let me know.


## Contributing
Pull requests that add support or documentation for more operating systems are
welcome.
