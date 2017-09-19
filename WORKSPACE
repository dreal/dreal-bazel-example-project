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
    commit = "4.17.09.1",
    sha256 = "83c8c5984f7487672da180723e070442a3cd8512837ae13db71d84673c6dbeaa",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
