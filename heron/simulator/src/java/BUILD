licenses(["notice"])

package(default_visibility = ["//visibility:public"])

load("/tools/rules/heron_deps", "heron_java_proto_files")

simulator_deps_files = \
    heron_java_proto_files() + [
        "//heron/api/src/java:api-java",
        "//heron/common/src/java:common-java",
        "@snakeyaml//jar",
    ]

java_library(
    name = "simulator-java",
    srcs = glob(["**/*.java"]),
    deps = simulator_deps_files, 
)
