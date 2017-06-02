# WarpWallet OSK

WarpWallet OSK is a slightly modified version of WarpWallet, which is developed by keybase. OSK stands for On-Screen Keyboard. WarpWallet OSK adds an on-screen keyboard (and that only) to the original WarpWallet in order to increase the security against keyloggers.

The official WarpWallet sites are:
https://github.com/keybase/warpwallet
https://keybase.io/warp/

The following part of this file is the same as the official version.

# warpwallet

A brain wallet generator that uses scrypt.

## Install

There's no npm module for WarpWallet since it's intended as a browser-only service.  However,
it does use npm to manage its dependencies

## Build

```sh
$ npm install -g iced-coffee-script
$ npm install -d
$ icake build
```

## Test

```sh
$ make test
```

## Regeneration of Test Vectors (which otherwise are fixed)

To generate our reference test vectors, we use the reference Scrypt implementation (in C), a 
Python PBKDF2, and a Python library to turn a seed into a keypair.  To see how this works, try:

```sh
$ cd test/gen && make build && make spec
```

## Why a Makefile and a Cakefile?

Internal disagreement as to which is better.





