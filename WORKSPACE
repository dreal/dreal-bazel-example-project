# -*- python -*-
workspace(name = "dreal_bazel_example")

load("//tools:github.bzl", "github_archive")

github_archive(
    name = "io_kythe_dreal", # Apache-2.0
    repository = "dreal-deps/kythe",
    commit = "beea4d79aac45e6a50774052254f8b74c4fa1b9c",
    sha256 = "81b93528a95f7ee60b2711cf46de8387018ba9d87ea568e8d347d337f3a1eb7b",
)

github_archive(
    name = "dreal", # Apache-2.0
    repository = "dreal/dreal4",
    commit = "4.17.10.1",
    sha256 = "1639781d8925d58d9d8413cd54696e8c10a0b65917328c7809b6531911a9c5d7",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
