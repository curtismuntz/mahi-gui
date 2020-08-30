#cc_library(
#    name = "mahi_color",
#    srcs = ["src/Mahi/Gui/Color.cpp"],
#    hdrs = ["include/Mahi/Gui/Color.hpp"],
#    includes = ["include"],
#    visibility = ["//visibility:public"],
#    deps = [
#        "//3rdparty/nanovg",
#        "@mahi_util",
#    ],
#)
#
#cc_library(
#    name = "mahi_vec2",
#    #    srcs = ["src/Mahi/Gui"],
#    hdrs = [
#        "include/Mahi/Gui/Detail/Vec2.inl",
#        "include/Mahi/Gui/Vec2.hpp",
#    ],
#    includes = ["include"],
#    visibility = ["//visibility:public"],
#)

cc_library(
    name = "mahi_gui",
    srcs = [
        "src/Mahi/Gui/Application.cpp",
        "src/Mahi/Gui/Color.cpp",
        "src/Mahi/Gui/Fonts/FontAwesome5.cpp",
        "src/Mahi/Gui/Fonts/FontAwesome5Brands.cpp",
        "src/Mahi/Gui/Fonts/RobotoBold.cpp",
        "src/Mahi/Gui/Fonts/RobotoItalic.cpp",
        "src/Mahi/Gui/Fonts/RobotoMonoBold.cpp",
        "src/Mahi/Gui/Fonts/RobotoMonoRegular.cpp",
        "src/Mahi/Gui/Fonts/RobotoRegular.cpp",
        "src/Mahi/Gui/Native.cpp",
        "src/Mahi/Gui/Shape.cpp",
        "src/Mahi/Gui/Transform.cpp",
        "src/Mahi/Gui/Transformable.cpp",
        "src/Mahi/Gui/imgui_custom.cpp",
        "src/Mahi/Gui/nanovg_custom.cpp",
    ],
    hdrs = glob([
        "include/Mahi/Gui/Detail/Tween.inl",
        "include/Mahi/Gui/Detail/Vec2.inl",
        "include/Mahi/Gui/Vec2.hpp",
        "include/Mahi/Gui/Color.hpp",
        "include/Mahi/Gui.hpp",
        "include/Mahi/Gui/Fonts.hpp",
        "include/Mahi/Gui/Application.hpp",
        "include/Mahi/Gui/Color.hpp",
        "include/Mahi/Gui/Coroutine.hpp",
        "include/Mahi/Gui/Fonts.hpp",
        "include/Mahi/Gui/imgui_custom.hpp",
        "include/Mahi/Gui/Macros.hpp",
        "include/Mahi/Gui/nanovg_custom.hpp",
        "include/Mahi/Gui/Native.hpp",
        "include/Mahi/Gui/Rect.hpp",
        "include/Mahi/Gui/Sequence.hpp",
        "include/Mahi/Gui/Shape.hpp",
        "include/Mahi/Gui/Transform.hpp",
        "include/Mahi/Gui/Transformable.hpp",
        "include/Mahi/Gui/Tween.hpp",
        "include/Mahi/Gui/Vec2.hpp",
        "include/Mahi/Gui.hpp",
        "include/Mahi/Gui/Icons/IconsFontAwesome5.hpp",
        "include/Mahi/Gui/Icons/IconsFontAwesome5Brands.hpp",
    ]),
    copts = [
        #        "-fcoroutines",
        "-std=c++14",
    ],
    includes = [
        "include",
        "include/Mahi",
        "include/Mahi/Gui/Detail",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//3rdparty/clipper",
        "//3rdparty/glad",
        "//3rdparty/glfw",
        "//3rdparty/imgui",
        "//3rdparty/implot",
        "//3rdparty/nanosvg",
        "//3rdparty/nanovg",
        "//3rdparty/nativefiledialog-extended:nfd",
        "@mahi_util",
    ],
)
