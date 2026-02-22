cc - C compiler
===============

An exercise in minimalism.

Try the following 
(If your system does not have "cc" use clang or gcc instead):

    mkdir -p build
    cc -o build/cc cc.c
    ./build/cc hello.c
    ./build/cc -s hello.c
    
    ./build/cc cc.c hello.c
    ./build/cc cc.c cc.c hello.c

Command Line Options
--------------------

    -s      dump source and assembly
    -d      dump debug execution trace
    --      end of options (pass remaining arguments to script)

Run tests:

    ./build/cc test/tests.c

Documentation
-------------

- [LANGUAGE.md](LANGUAGE.md) - EBNF grammar and supported C99 features

