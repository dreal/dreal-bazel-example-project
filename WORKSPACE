# -*- python -*-
workspace(name = "dreal_bazel_example")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

DREAL_COMMIT = "2ecbc869a10f51be32670467c1bcd54a43a002dd"

DREAL_SHA256 = "11c47f34a45e3aa80dc8cf83c1db9a31f033c035e1e22cfc42dce69cc33fa546"

http_archive(
    name = "dreal",  # Apache-2.0
    sha256 = DREAL_SHA256,
    strip_prefix = "dreal4-{}".format(DREAL_COMMIT),
    urls = [
        "https://github.com/dreal/dreal4/archive/{}.tar.gz".format(DREAL_COMMIT),
    ],
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")

dreal_workspace()
