local_repository(
    name = "mahi_util",
    path = "/home/murt/murt/open_source/mahi-util",
)

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

#http_archive(
#    name = "mahi_util",
#    urls = ["https://github.com/curtismuntz/mahi-util/archive/96e4e1d334b289f74174009bc02ccb3df12463d0.tar.gz"],
#    strip_prefix = "mahi-util-96e4e1d334b289f74174009bc02ccb3df12463d0",
#    sha256 = "d2f49abf35fb9de826469dfd66c347dd7fc0e6824041b4dfc3a48fd9f47878bf",
#)

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
