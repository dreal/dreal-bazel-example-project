# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.18.10.1",
    sha256 = "919db0574c3488e4a744181bf3b480f827756c9528cbe2f0c7ffa29f2ebf89e8",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
