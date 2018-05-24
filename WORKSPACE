# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.18.05.2",
    sha256 = "6919b8cb233f6228f27f913327db16de75c5b154f9de8207aac3eaa0db0a316d",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
