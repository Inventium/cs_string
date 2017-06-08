## CsString

### Introduction

CsString is a standalone library which provides unicode aware string support.

The CsBasicString class is a templated class which provides unicode aware string support. The encoding, such
as UTF-8 or UTF-16, is passed to the CsBasicString template. The following typedefs are provided for convenience.

    using CsString       = CsBasicString<utf8>;
    using CsString_utf8  = CsBasicString<utf8>;
    using CsString_utf16 = CsBasicString<utf16>;

### System Requirements

To use CsString you will need a C++11 compiler and a C++11 standard library.

Currently uses the Autotools build system for building and running the unit test suite.
The library has been tested with clang sanitizer and a major code review.

#### Building on (modern) OSX

If you want to build on OSX, you have probably already figured out that
there is no home brew available. But that's ok, use home brew to install
autotools and an up-to-date gcc. Once autotools is installed:

    $ glibtoolize
    $ autoreconf
    $ ./configure --prefix=$HOME/lib
    $ make && make install

Once it's finished compiling, you should find

    $ ls bin/lib/
    libCsString.0.dylib  libCsString.dylib  libCsString.la

There is no static link at the moment.

### Documentation

Class level documentation for CsString is available on the CopperSpice website:

www.copperspice.com/docs/cs_string/index.html


### Presentations

For additional information refer to our CsString presentations at CppCon 2017:

www.copperspice.com/presentations.html


### Authors

* **Ansel Sermersheim**
* **Barbara Geller**


### License

This library is released under the BSD 2-clause license. For more information refer to the
LICENSE file provided with this project. 


### References

* Website: www.copperspice.com
* Email:   info@copperspice.com










