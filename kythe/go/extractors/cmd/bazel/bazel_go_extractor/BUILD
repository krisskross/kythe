load("//tools:build_rules/shims.bzl", "go_binary")

package(default_visibility = ["//kythe:default_visibility"])

go_binary(
    name = "bazel_go_extractor",
    srcs = ["bazel_go_extractor.go"],
    deps = [
        "//kythe/go/extractors/bazel",
        "//kythe/go/extractors/golang",
        "//kythe/go/extractors/govname",
        "//kythe/go/util/vnameutil",
        "//kythe/proto:analysis_go_proto",
        "//kythe/proto:go_go_proto",
        "//kythe/proto:storage_go_proto",
        "//third_party/bazel:extra_actions_base_go_proto",
        "@com_github_golang_protobuf//proto:go_default_library",
        "@org_bitbucket_creachadair_shell//:go_default_library",
        "@org_bitbucket_creachadair_stringset//:go_default_library",
    ],
)
