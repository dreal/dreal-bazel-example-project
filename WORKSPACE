# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "io_kythe", # Apache-2.0
    repository = "dreal-deps/kythe",
    commit = "749b36e4249250710bd8f29f26c7cb2e720562bc",
    sha256 = "87ff317ab7ac658eb48f2c0abdd9f407bf4f1b87b8bff6e15bf3f56d54548975",
)

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal3-apache2",
    commit = "07a1403c947b90f3228625698db2ffb7eb7bc7ba",
    sha256 = "c85d43a00d60efb17c592dc151f97bb3401f57cc35d4b2b6d893e9071cc4b981",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
