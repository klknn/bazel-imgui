load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive", "http_file")

http_archive(
    name = "imgui",
    url = "https://github.com/ocornut/imgui/archive/refs/tags/v1.89.8.zip",
    strip_prefix = "imgui-1.89.8",
    build_file = "@//third_party:BUILD.imgui",
    sha256 = "16b9d46385fb38340691c4dce7cf4547b161866f9c85fa588293df27e1667bfd",
)

http_archive(
    name = "glfw_macos",
    url = "https://github.com/glfw/glfw/releases/download/3.3.8/glfw-3.3.8.bin.MACOS.zip",
    strip_prefix = "glfw-3.3.8.bin.MACOS",
    build_file = "@//third_party:BUILD.glfw",
    sha256 = "dc1fc3d3e7763b9de66f7cbb86c4ba3a82118441a15f64045a61cfcdedda88d2",
)

http_archive(
    name = "glfw_win64",
    url = "https://github.com/glfw/glfw/releases/download/3.3.8/glfw-3.3.8.bin.WIN64.zip",
    strip_prefix = "glfw-3.3.8.bin.WIN64",
    build_file = "@//third_party:BUILD.glfw",
    sha256 = "7851c068b63c3cebf11a3b52c9e7dbdb6159afe32666b0aad268e4a258a9bdd1",
)

http_archive(
    name = "glfw_src",
    url = "https://github.com/glfw/glfw/releases/download/3.3.8/glfw-3.3.8.zip",
    strip_prefix = "glfw-3.3.8",
    build_file = "//third_party:BUILD.glfw_src",
    sha256 = "4d025083cc4a3dd1f91ab9b9ba4f5807193823e565a5bcf4be202669d9911ea6",
)

# In linux, you can use this instead of `glfw_src` after `apt install libglfw3-dev`.
# Replace @glfw_src//:glfw in //third_party/BUILD.imgui with @glfw_linux//:glfw_linux.
new_local_repository(
    name = "glfw_linux",
    path = "/usr",
    build_file = "//third_party:BUILD.glfw"
)
