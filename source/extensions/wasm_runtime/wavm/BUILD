load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_extension",
    "envoy_extension_package",
)

licenses(["notice"])  # Apache 2

envoy_extension_package()

envoy_cc_extension(
    name = "config",
    srcs = ["config.cc"],
    security_posture = "unknown",
    status = "alpha",
    deps = [
        "//include/envoy/registry",
        "//source/extensions/common/wasm:wasm_lib",
    ],
)
