This development project aggregates Boost.Reflect, Boost.CMT, 
Boost.RPC and their non-standard dependenices Boost.Context, 
Boost.Move, Boost.Atomic into a single project.

### Installation ## 

    git clone https://github.com/bytemaster/dev
    cd dev
    git submodule init
    git submodule update
    cmake .
    make
    make install
    @endcode


### Notice ###

    These libraries are not part of the official Boost C++ library, but
    is written, to the best of my ability, to follow the best practices
    established by the Boost community and with the hope of being 
    considered for inclusion with a future Boost release.
