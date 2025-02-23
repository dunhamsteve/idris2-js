
# Idris2 for Node

This repository patches and builds the Idris2 compiler for nodejs. It is intended for use on small memory systems that can't build the full chez version.  There are some stack issues when building larger programs. 


## Installation

- Download the `idris2-js.zip` file for the release.
- Unzip and move `.idris2-js` to your home directory
- Add `~/.idris2-js` to your `PATH`

If you place it elsewhere or rename it, the environment variable `IDRIS2_PREFIX` should point to what was the `.idris2-js` directory.

- REPL and command line work
- IDE mode is disabled (TODO)
- `node` is the default codegen

The patches are found in `Node.patch`, and the build script is `BUILDJS`.

## Running with bun

If you have [bun](https://bun.sh/) installed. You will get fewer stack overflows if you replace `node` with `bun run` on the first line of `~/.idris2-js/bin/idris2`.
