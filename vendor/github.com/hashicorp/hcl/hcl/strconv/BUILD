load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["quote.go"],
    importpath = "github.com/hashicorp/hcl/hcl/strconv",
    visibility = ["//visibility:public"],
)

go_test(
    name = "go_default_test",
    srcs = ["quote_test.go"],
    importpath = "github.com/hashicorp/hcl/hcl/strconv",
    library = ":go_default_library",
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
