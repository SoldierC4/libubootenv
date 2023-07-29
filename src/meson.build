install_headers('libuboot.h')

libubootenv_lib = library(
  'ubootenv',
  'uboot_env.c',
  version: meson.project_version(),
  dependencies: [yaml_dep, zlib_dep],
  install: true
)

fw_printenv = executable(
  'fw_printenv',
  'fw_printenv.c',
  link_with: libubootenv_lib,
  install: true
)

fw_setenv = executable(
  'fw_setenv',
  'fw_printenv.c',
  link_with: libubootenv_lib,
  install: true
)
