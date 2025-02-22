
# Idris2 for Node

This repository patches and builds the Idris2 compiler for nodejs. It is intended for use on small memory systems that can't build the full chez version.


## Installation

- Download the zipfile for the release.
- unzip and move `.idris2-js` to your home directory
- add `~/.idris2-js` to your `PATH`

If you place it elsewhere or rename it, the environment variable `IDRIS2_PREFIX` should point to what was the `.idris2-js` directory.

- REPL and command line work
- IDE mode is disabled (TODO)
- `node` is the default codegen

The patches are in `Node.patch`, the build script is `BUILDJS`.
