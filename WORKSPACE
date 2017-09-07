# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "io_kythe_dreal", # Apache-2.0
    repository = "dreal-deps/kythe",
    commit = "333ddf386fda81fb3f9962e54eb30a67b14315db",
    sha256 = "63d59334434f6d84c89da46d04305736fa58c29282f9d9372580dc0957a61b70",
)

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "173699a48878fe773ee2ded09b2559a11954aaf8",
    sha256 = "e1e95572cf85c0d1d3478de18c3774d3ff055e75da9ce74fb53b203711cb889c",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
