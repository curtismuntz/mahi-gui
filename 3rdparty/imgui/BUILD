cc_library(
    name = "imgui",
    srcs = [
        "examples/imgui_impl_glfw.cpp",
        "examples/imgui_impl_opengl3.cpp",
        "imgui.cpp",
        "imgui.h",
        "imgui_demo.cpp",
        "imgui_draw.cpp",
        "imgui_stdlib.cpp",
        "imgui_widgets.cpp",
    ],
    hdrs = [
        #    "imconfig.h", # depends on a bunch of stuff that'd make a circular dep
        "imgui_internal.h",
        "imgui.h",
        "imstb_rectpack.h",
        "imstb_textedit.h",
        "imstb_truetype.h",
        "imgui_stdlib.h",
        "examples/imgui_impl_glfw.h",
        "examples/imgui_impl_opengl3.h",
    ],
    defines = ["IMGUI_DISABLE_INCLUDE_IMCONFIG_H"],
    includes = [
        ".",
        "examples",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//3rdparty/glad",
        "//3rdparty/glfw",
        "//3rdparty/nanovg",
    ],
)

cc_binary(
    name = "example",
    srcs = [
        "examples/example_glfw_opengl3/main.cpp",
    ],
    linkopts = [
        "-ldl",
        "-lX11",
        "-lpthread",
    ],
    local_defines = ["IMGUI_IMPL_OPENGL_LOADER_GLAD"],
    deps = [
        #        ":example_lib",
        ":imgui",
        "//3rdparty/glfw",
    ],
)
