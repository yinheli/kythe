load("//tools:build_rules/shims.bzl", "go_test", "go_library")

package(default_visibility = ["//kythe:default_visibility"])

go_library(
    name = "compare",
    srcs = ["compare.go"],
    deps = [
        "//kythe/proto:storage_go_proto",
        "@com_github_golang_protobuf//proto:go_default_library",
        "@com_github_google_go_cmp//cmp:go_default_library",
    ],
)

go_test(
    name = "compare_test",
    srcs = ["compare_test.go"],
    library = "compare",
)
