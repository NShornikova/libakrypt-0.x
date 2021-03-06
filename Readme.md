# Libakrypt

Libakrypt is a free and open source library (crypto module) for OpenSKZI project
distributed under the 3-clause BSD License.
This library written in C11 and provides some interfaces for
key management, data encryption, integrity checking, signing messages and
verifying of digital signatures. The main goal of Libakrypt
is implementation of many Russian crypto mechanisms, decribed by national
standards and methodological recomendations.

We have implementation of:
 - GOST R 34.12-2015 block ciphers "Magma" & "Kuznechik" with 64 bit and 128 bit
   block sizes respectively;
 - GOST R 34.13-2015 modes for block ciphers;
 - GOST R 34.11-2012 & GOST R 34.11-94 hash functions;
 - GOST R 34.10-2012 digital signature algorithms;
 - R 50.1.113-2016 crypto algorithms such as HMAC;
 - a some set of pseudo random generators for various operation systems.

We hope that libakrypt can be used successfully
under Linux, Windows (since XP), FreeBSD, MacOs and ReactOS operation systems.

## Compilation

The library can be compiled with many compilers,
such as gcc, clang, Microsoft Visual C, TinyCC and icc.
You can get the last version of source codes from github.com

    git clone https://github.com/axelkenzo/libakrypt-0.x

The build system for libakrypt is [cmake](https://cmake.org/).

### Unix
On Unix platforms you can compile & build library with following commands

    mkdir build
    cd build
    cmake ../libakrypt-0.x
    make

### Windows
On Windows you need to install [phtreads library](https://sourceware.org/pthreads-win32/).
After this you can run a Microsoft Visual 20XX Console and execute a following sequence

    mkdir build
    cd build
    cmake.exe -G "NMake Makefiles" ../libakrypt-0.x
    nmake.exe

The full list of compile & build options you can find
in documentation, see libakrypt-doc-0.x.pdf (in russian).

## Attention

Since this version still under development we don't recomended to use it
in real security applications.

