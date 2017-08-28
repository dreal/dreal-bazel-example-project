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
    commit = "319cd5f5523a7ecdbf40132252c5c77f792e2c6b",
    sha256 = "ba2b57bc61b92d81b031cc87862ad59570e2b86a907f0182877813ab2a0c20b1",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
