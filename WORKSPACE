# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.18.03.1",
    sha256 = "02051d9695a7395d25135901ddc1203449bf45ac653069452f43e9d615fb248e",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
