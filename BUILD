cc_library(
    name = "mahi_color",
    srcs = ["src/Mahi/Gui/Color.cpp"],
    hdrs = ["include/Mahi/Gui/Color.hpp"],
    includes = ["include"],
    visibility = ["//visibility:public"],
    deps = [
        "//3rdparty/nanovg",
        "@mahi_util",
    ],
)

cc_library(
    name = "mahi_vec2",
    #    srcs = ["src/Mahi/Gui"],
    hdrs = [
        "include/Mahi/Gui/Detail/Vec2.inl",
        "include/Mahi/Gui/Vec2.hpp",
    ],
    includes = ["include"],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "mahi_gui",
    srcs = glob(["src/Mahi/Gui/**/*.cpp"]),
    hdrs = glob([
        "include/Mahi/**/*.hpp",
        "include/Mahi/**/*.inl",
    ]),
    copts = [
        "-fcoroutines",
        "-std=c++2a",
    ],
    includes = ["include"],
    visibility = ["//visibility:public"],
)
