An example [bazel](https://bazel.build/) project to show you how to
use dReal as a library in a bazel project.

[![Build Status](https://travis-ci.org/dreal/dreal-bazel-example-project.svg?branch=master)](https://travis-ci.org/dreal/dreal-bazel-example-project)

Setup
=====

You need to have the dependencies of
[dReal4](https://github.com/dreal/dreal4) installed in your system.

macOS 10.12/10.13
-----

We use [homebrew](https://brew.sh).

```bash
brew install bazel pkg-config dreal-deps/ibex/ibex nlopt
```


Ubuntu 14.04/16.04
------------------

```bash
sudo apt install -y software-properties-common  # for add-apt-repository
sudo add-apt-repository ppa:dreal/dreal -y
sudo apt update
sudo apt install bison coinor-libclp-dev flex pkg-config libibex-dev libnlopt-dev
```


Bazel Build
===========

Following the above setup, please run the following to build and run
the example project.

```bash
git clone https://github.com/dreal/dreal-bazel-example-project.git
cd dreal-bazel-example-project
bazel build //...
./bazel-bin/check_sat
```
