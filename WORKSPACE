workspace(name = "differentialPrivacyR")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository", "new_git_repository")

local_repository(
    name = "google_dp",
    path = "src/differential_privacy",
)

git_repository(
    name = "com_google_absl",
    commit = "aae8143cf9aa611f70d7ea9b95b8b8b383b2271a",
    remote = "https://github.com/abseil/abseil-cpp",
)

http_archive(
            name = "com_google_protobuf",
            urls = ["https://github.com/protocolbuffers/protobuf/archive/v3.8.0.tar.gz"],
            sha256 = "03d2e5ef101aee4c2f6ddcf145d2a04926b9c19e7086944df3842b1b8502b783",
            strip_prefix = "protobuf-3.8.0",
        )