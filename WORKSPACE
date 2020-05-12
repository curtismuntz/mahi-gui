local_repository(
    name = "mahi_util",
    path = "/home/murt/murt/opensource/mahi-util",
)

new_local_repository(
    name = "gtk_headers",
    build_file_content = """
package(default_visibility = ["//visibility:public"])
cc_library(
    name = "headers",
    hdrs = glob(["**/*.h"])
)
""",
    path = "/usr/lib/x86_64-linux-gnu/gtk-3.0",
)

new_local_repository(
    name = "glib_headers",
    build_file_content = """
package(default_visibility = ["//visibility:public"])
cc_library(
    name = "headers",
    hdrs = glob(["**/*.h"])
)
""",
    path = "/usr/lib/x86_64-linux-gnu/glib-2.0/include",
)
