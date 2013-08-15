# libLBFGS

C library of limited-memory BFGS (L-BFGS)

libLBFGS is a C port of the implementation of Limited-memory
[Broyden-Fletcher-Goldfarb-Shanno](http://en.wikipedia.org/wiki/BFGS_method) (L-BFGS) method written by Jorge Nocedal.
The original FORTRAN source code is available [here](http://www.ece.northwestern.edu/~nocedal/lbfgs.html).

The L-BFGS method solves the unconstrained minimization problem:

    minimize F(x), x = (x1, x2, ..., xN)

only if the objective function `F(x)` and its gradient `G(x)` are computable.

Refer to the [libLBFGS web site](http://www.chokkan.org/software/liblbfgs/) for more information.

## Installation

    git clone https://github.com/chbrown/liblbfgs
    ./configure
    make
    make install

Or you might need to bump up your permissions:

    sudo make install

This will produce the following files (depending on your system's build defaults):

    /usr/local/include/lbfgs.h
    /usr/local/lib/liblbfgs.a
    /usr/local/lib/liblbfgs.la
    /usr/local/lib/liblbfgs-1.10.so
    /usr/local/lib/liblbfgs.so -> liblbfgs-1.10.so
    /usr/local/share/doc/liblbfgs/*

More documentation about the configuration settings can be found in []().

## License

libLBFGS is distributed under the terms of the [MIT license](COPYING).

Copyright (c) 1990, Jorge Nocedal
Copyright (c) 2007-2010, Naoaki Okazaki
