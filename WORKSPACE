# -*- python -*-
workspace(name = "dreal_bazel_example")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

DREAL_COMMIT = "master"

DREAL_SHA256 = ""

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
