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

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal3-apache2",
    commit = "b13eb8283b42e4f4eec96695813df03eefcd0453",
    sha256 = "e45b6bb91dc99545847e49994fb6fbac49527ffcecc41bea4c7981573519583e",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
