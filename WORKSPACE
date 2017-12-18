# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "io_kythe_dreal", # Apache-2.0
    commit = "ee2e00de4b72e9ed9f1b819898b5238c03d10dd6",
    repository = "dreal-deps/kythe",
    sha256 = "7229c5d5a471fd26bcc50b5202568dc9c3035d7375312eb92ded9230e9f6886f",
)

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "5ee74add52a726de12f54be536621df69051d1d9",
    sha256 = "f3c0d9e55b71311397a71c2a61b0053ffd1916cea21e5ddc2d941efd35c00aaf",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
