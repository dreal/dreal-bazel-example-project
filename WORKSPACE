# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "8e78a9b5434114abca24a9e949686861beea40e0",  # 4.18.10.1 + custom
    sha256 = "268a986bd2ec7024e35267a2a47afc42bd09803df30106a340fed33571cafa57",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
