package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "clientset.go",
        "doc.go",
        "import_known_versions.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//federation/apis/federation/install:go_default_library",
        "//federation/client/clientset_generated/federation_clientset/typed/autoscaling/v1:go_default_library",
        "//federation/client/clientset_generated/federation_clientset/typed/batch/v1:go_default_library",
        "//federation/client/clientset_generated/federation_clientset/typed/core/v1:go_default_library",
        "//federation/client/clientset_generated/federation_clientset/typed/extensions/v1beta1:go_default_library",
        "//federation/client/clientset_generated/federation_clientset/typed/federation/v1beta1:go_default_library",
        "//pkg/client/typed/discovery:go_default_library",
        "//vendor:github.com/golang/glog",
        "//vendor:k8s.io/client-go/pkg/util/flowcontrol",
        "//vendor:k8s.io/client-go/plugin/pkg/client/auth",
        "//vendor:k8s.io/client-go/rest",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//federation/client/clientset_generated/federation_clientset/fake:all-srcs",
        "//federation/client/clientset_generated/federation_clientset/typed/autoscaling/v1:all-srcs",
        "//federation/client/clientset_generated/federation_clientset/typed/batch/v1:all-srcs",
        "//federation/client/clientset_generated/federation_clientset/typed/core/v1:all-srcs",
        "//federation/client/clientset_generated/federation_clientset/typed/extensions/v1beta1:all-srcs",
        "//federation/client/clientset_generated/federation_clientset/typed/federation/v1beta1:all-srcs",
    ],
    tags = ["automanaged"],
)
