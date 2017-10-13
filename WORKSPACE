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
    commit = "4.17.10.2",
    sha256 = "e02d1073cc1594b9f0a4ac949db0fcd2b0a3879d9db69e8d5266e2547634680b",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
