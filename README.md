# bazel-imgui

1. Install bazelisk prebuilt binary as bazel https://github.com/bazelbuild/bazelisk/releases
2. Run this command to check its working: `bazel run :example_glfw_opengl3`
3. Copy WORKSPACE and third_party/BUILD.imgui in your bazel project.

## History

- 2023/08/23: Added GLFW+OpenGL3 example for win/osx (using the official binary) and linux (using the official source and `apt install libx11-dev libxi-dev libxinerama-dev libxcursor-dev`).
- 2023/08/22: Added win32 backends.
