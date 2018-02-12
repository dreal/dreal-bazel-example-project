# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.18.02.2",
    sha256 = "51f576a8881d3f916293b2ff56dc7038638e694a6ed6da9c1503cf0e37957d0d",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
