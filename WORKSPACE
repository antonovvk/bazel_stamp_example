# bazel_stamp repository
git_repository(
    commit = "a331398d4d6dfec649e377e75b7c138c337fd86f",
    name = "com_github_antonovvk_bazel_stamp",
    remote = "https://github.com/antonovvk/bazel_stamp",
)

# GoLang-only workspace deps
git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go",
    tag = "0.12.1",
)

git_repository(
    name = "bazel_skylib",
    remote = "https://github.com/bazelbuild/bazel-skylib",
    tag = "0.2.0",
)

git_repository(
    name = "bazel_gazelle",
    remote = "https://github.com/bazelbuild/bazel-gazelle",
    tag = "0.12.0",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")
go_rules_dependencies()
go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")
gazelle_dependencies()
