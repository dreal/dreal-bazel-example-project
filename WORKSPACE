# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.18.02.3",
    sha256 = "23d364d393d8ccde14e7f9ca9c1b19c97a7f97d54a4c2b15ef1ffaa2c80dccf3",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
