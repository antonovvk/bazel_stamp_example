load("@com_github_antonovvk_bazel_stamp//:stamp.bzl", "cc_stamp")

cc_stamp(
    name = "stamp",
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "cc_stamp",
    srcs = ["main.cpp"],
    copts = [
        "-std=c++11",
        "-Wall",
    ],
    stamp = 1,
    visibility = ["//visibility:public"],
    deps = ["stamp"],
)
