# Generated by Buckaroo - https://buckaroo.pm
include_defs('//BUCKAROO_DEPS')

cxx_library(
  name = 'rxterm',
  header_namespace = 'rxterm',
  srcs = glob([
    'rxterm/src/**/*.cpp',
  ]),
  headers = subdir_glob([
    ('rxterm/detail', '**/*.h'),
    ('rxterm/detail', '**/*.hpp'),
  ]),
  exported_headers = subdir_glob([
    ('rxterm/include', '**/*.h'),
    ('rxterm/include', '**/*.hpp'),
  ]),
  deps = BUCKAROO_DEPS,
  licenses = [
    'LICENSE',
  ],
  visibility = [
    'PUBLIC'
  ],
)

cxx_binary(
  name = 'main',
  srcs = [
    'rxterm/apps/main.cpp'
  ],
  deps = [
    ':rxterm',
  ],
)
