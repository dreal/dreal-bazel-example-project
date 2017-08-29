# -*- python -*-
workspace(name = "dreal_bazel_example")

local_repository(
    name = "kythe",
    path = "tools/third_party/kythe",
)

load("@kythe//tools/build_rules/config:pkg_config.bzl", "pkg_config_package")

pkg_config_package(
    name = "ibex",
    modname = "ibex",
)

pkg_config_package(
    name = "clp",
    modname = "clp",
)

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal3-apache2",
    commit = "b3b5a106ab132126c5d67a4be4e073108d1d035e",
    sha256 = "49b210b61a4eaee641675a3daa1cf9457148600847b22032af0162201a7f00fe",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
