GENERIC_SRCS = [
    "src/internal.h",
    "src/mappings.h",
    "src/context.c",
    "src/init.c",
    "src/input.c",
    "src/monitor.c",
    "src/vulkan.c",
    "src/window.c",
]

WAYLAND_SRCS = [
    "src/wl_platform.h",
    "src/posix_time.h",
    "src/posix_thread.h",
    "src/xkb_unicode.h",
    "src/egl_context.h",
    "src/osmesa_context.h",
    "src/wl_init.c",
    "src/wl_monitor.c",
    "src/wl_window.c",
    "src/posix_time.c",
    "src/posix_thread.c",
    "src/xkb_unicode.c",
    "src/egl_context.c",
    "src/osmesa_context.c",
]

X11_SRCS = [
    "src/x11_platform.h",
    "src/xkb_unicode.h",
    "src/posix_time.h",
    "src/posix_thread.h",
    "src/glx_context.h",
    "src/egl_context.h",
    "src/osmesa_context.h",
    "src/x11_init.c",
    "src/x11_monitor.c",
    "src/x11_window.c",
    "src/xkb_unicode.c",
    "src/posix_time.c",
    "src/posix_thread.c",
    "src/glx_context.c",
    "src/egl_context.c",
    "src/osmesa_context.c",
]

X11_OR_WAYLAND_SRCS = [
    "src/linux_joystick.c",
    "src/linux_joystick.h",
]

cc_library(
    name = "glfw",
    srcs = GENERIC_SRCS + X11_SRCS + X11_OR_WAYLAND_SRCS,
    hdrs = [
        "include/GLFW/glfw3.h",
        "include/GLFW/glfw3native.h",
    ],
    defines = [
        #        "_GLFW_WAYLAND"
        "_GLFW_X11",
    ],
    #    include_prefix = "GLFW",
    includes = ["include"],
    #    includes = ["."],
    linkopts = [
        "-lrt",
        "-lm",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//3rdparty/glad",
        "//3rdparty/nanovg",
    ],
)
