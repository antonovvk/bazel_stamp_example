load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")

go_binary(
    name = "go_stamp",
    embed = [":go_default_library"],
    visibility = ["//visibility:public"],
)

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    importpath = "github.com/antonovvk/bazel_stamp_example/go_stamp",
    visibility = ["//visibility:private"],
    deps = ["@com_github_antonovvk_bazel_stamp//go:go_default_library"],
)
