# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "2ecbc869a10f51be32670467c1bcd54a43a002dd",  # 4.18.11.4
    sha256 = "11c47f34a45e3aa80dc8cf83c1db9a31f033c035e1e22cfc42dce69cc33fa546",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
