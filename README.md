## Reason: simple, fast & type safe code that leverages the JavaScript & OCaml ecosystems

[![Build Status](https://travis-ci.org/facebook/reason.svg?branch=master)](https://travis-ci.org/facebook/reason) [![CircleCI](https://circleci.com/gh/facebook/reason/tree/master.svg?style=svg)](https://circleci.com/gh/facebook/reason/tree/master)

### [Getting Started](https://reasonml.github.io/guide/javascript/quickstart)

### [Community](https://reasonml.github.io/community/)

## Contributing

### Documentations

The doc repo lives at https://github.com/reasonml/reasonml.github.io

### Codebase

See the [src folder](ttps://github.com/facebook/reason/tree/master/src) and the corresponding README.

```
# On OSX, install opam via Homebrew:
brew update
brew install opam
# On Linux, see here (you will need opam >= 1.2.2): http://opam.ocaml.org/doc/Install.html

opam init
# Add this to your ~/.bashrc (or ~/.zshrc), then do `source ~/.bashrc`
#   eval $(opam config env)

opam update
opam switch 4.04.1
eval $(opam config env)
git clone https://github.com/facebook/reason.git
cd reason
opam pin add -y reason .
```

**Note**: during the last `opam pin` step, make sure your local repo is clean. In particular, remove artifacts and `node_modules`. Otherwise the pinning might go stale or stall due to the big `node_modules`.

### Build

`make build`. **If this fails on your machine but master passes**, it means your setup wasn't right. Could you check if you followed the above installation steps? In particular, make sure you did `eval $(opam config env)` and sourced your shell environment (if you don't know how, just open a new shell tab and it'll be sourced usually).

### Test

`make test` (make sure to follow the repo pinning instructions above!)

## License

See Reason license in [LICENSE.txt](LICENSE.txt).

Works that are forked from other projects are under their original licenses.

Editor plugins (which have also been forked) in the `editorSupport/` directory include their own licenses.

## Credit

The general structure of `refmt` repo was copied from @whitequark's m17n project, including parts of the `README` that instruct how to use this with the OPAM toolchain.
