[![Build Status](https://travis-ci.org/dreal/dreal-bazel-example-project.svg?branch=master)](https://travis-ci.org/dreal/dreal-bazel-example-project)

An example [bazel](https://bazel.build/) project to show you how to
use dReal as a library in a bazel project.

Setup
=====

Install [the prerequsites to build dReal](https://github.com/dreal/dreal4#install-prerequsites).

Build Example Project
=====================

Following the above setup, please run the following to build and run
the example project.

```bash
git clone https://github.com/dreal/dreal-bazel-example-project.git
cd dreal-bazel-example-project
bazel build //...
./bazel-bin/check_sat
```
