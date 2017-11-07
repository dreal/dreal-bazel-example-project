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
    commit = "13c47fb8cbbf26764fbb215217020ec484d68940",
    sha256 = "ab1781a19a3d9d52e19d00f8da3a163093c863257abbb04f160cb3dc15cd9aa3",
)

load("@dreal//dreal:workspace.bzl", "dreal_workspace")
dreal_workspace()
