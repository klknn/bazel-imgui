load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "imgui",
    url = "https://github.com/ocornut/imgui/archive/refs/tags/v1.89.8.zip",
    strip_prefix = "imgui-1.89.8",
    build_file = "@//third_party:BUILD.imgui",
    workspace_file = "@//third_party:WORKSPACE.imgui",
)

http_archive(
    name = "glfw_macos",
    url = "https://github.com/glfw/glfw/releases/download/3.3.8/glfw-3.3.8.bin.MACOS.zip",
    strip_prefix = "glfw-3.3.8.bin.MACOS",
    build_file = "@//third_party:BUILD.glfw",
)
