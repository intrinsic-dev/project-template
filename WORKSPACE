workspace(name="project-template")

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

git_repository(
    name = "ai_intrinsic_sdks",
    remote = "https://github.com/intrinsic-dev/intrinsic_sdks",
    tag = "intrinsic.platform.20230612.RC11",
)

# Load shared dependencies for Intrinsic SDKs. None of these is optional.
load("@ai_intrinsic_sdks//bazel:deps_0.bzl", "intrinsic_sdks_deps_0")
intrinsic_sdks_deps_0()
load("@ai_intrinsic_sdks//bazel:deps_1.bzl", "intrinsic_sdks_deps_1")
intrinsic_sdks_deps_1()
load("@ai_intrinsic_sdks//bazel:deps_2.bzl", "intrinsic_sdks_deps_2")
intrinsic_sdks_deps_2()
load("@ai_intrinsic_sdks//bazel:deps_3.bzl", "intrinsic_sdks_deps_3")
intrinsic_sdks_deps_3()


# Python PIP dependencies
# To obtain requirements.txt file please run in VS Code terminal
#   pip-compile requirements.in
# To enabled Python PIP dependencies in your project,
# please uncomment following  lines
#
# load("@rules_python//python:pip.bzl", "pip_parse")
# load("@ai_intrinsic_sdks//bazel:python.bzl", "interpreter")
#
# pip_parse(
#     # You can choose a name under which to reference your PIP dependencies.
#     name = "project_pip_deps",
#     python_interpreter_target = interpreter,
#     requirements_lock = "//:requirements.txt",
# )
#
# load("@project_pip_deps//:requirements.bzl", "install_deps")
#
# install_deps()
