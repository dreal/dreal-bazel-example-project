# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.18.02.1",
    sha256 = "6f8a8d3f6f77612953231203e312b9ada94946042f1e4c65016d8bef954757ae",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
