# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "io_kythe_dreal", # Apache-2.0
    repository = "dreal-deps/kythe",
    commit = "333ddf386fda81fb3f9962e54eb30a67b14315db",
    sha256 = "9e8db92c3eb605be5a74daf6f0621298a487b6b2e4f279e68ddf8b513826491b",
)

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "5421fa080416f90c1d79c4c47a900031acacacfb",
    sha256 = "e6d744591defa82edc7107544ce12142c9ab74bea5386229ed2ab2afb242c44d",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
