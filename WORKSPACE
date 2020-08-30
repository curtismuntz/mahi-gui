#local_repository(
#    name = "mahi_util",
#    path = "/home/murt/murt/opensource/mahi-util",
#)
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "mahi_util",
    urls = ["https://github.com/curtismuntz/mahi-util/archive/ebd1fc92b5dd9d601e7ceff38cc3e9b0daa4cd42.tar.gz"],
    strip_prefix = "mahi-util-ebd1fc92b5dd9d601e7ceff38cc3e9b0daa4cd42",
    sha256 = "d2f49abf35fb9de826469dfd66c347dd7fc0e6824041b4dfc3a48fd9f47878bf",
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
