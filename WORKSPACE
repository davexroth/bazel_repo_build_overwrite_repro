workspace(name = "overwrite")

new_local_repository(
    name = "contents",
    path = "external/contents",
    build_file_content =
  """
cc_library(
    name = "a",
    hdrs = [
        "a.h",
    ],
    visibility = ["//visibility:public"],
)
  """
)

new_local_repository(
    name = "file",
    path = "external/file",
    build_file = "file.BUILD.bazel"
)
