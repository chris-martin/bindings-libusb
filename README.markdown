Low level bindings to
[libusb-1.*](http://libusb.sourceforge.net/api-1.0/)

This package uses
[bindings-DSL](http://hackage.haskell.org/package/bindings-DSL) and
conforms to its naming convention.

For a higher-level and more Haskell friendly binding (which uses this
package) see the [usb](http://hackage.haskell.org/package/usb)
package.

# Installing

Make sure the `libusb` C library is installed:

* *Ubuntu Linux*: `sudo apt-get install libusb-1.0-0-dev`
* *Gentoo Linux*: `sudo emerge libusb`
* *MS Windows*:
    [Download `libusb` for MS Windows](http://www.libusb.org/wiki/windows_backend#LatestBinarySnapshots)
     and extract it somewhere e.g. `C:\Program Files\libusb\libusb1`.

    Important build-time files: `libusb-1.0\include\libusb.h` and
    `MinGW32\dll\libusb-1.0.dll.a`

    Important run-time files: `MinGW32\dll\libusb-1.0.dll`

    Make sure to use the following cabal options:

        --extra-include-dirs="C:\Program Files\libusb\libusb1\include\libusb-1.0"

        --extra-lib-dirs="C:\Program Files\libusb\libusb1\MinGW32\dll"
