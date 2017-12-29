project(
  'termbox', 'c'
, default_options : [
    'c_std=gnu99'
  , 'warning_level=3'
  , 'werror=true'
  ]
)

termbox_exported = declare_dependency(
  include_directories : include_directories('src')
, link_with : static_library(
    'termbox'
  , ['src/termbox.c', 'src/utf8.c']
  , c_args : '-D_XOPEN_SOURCE'
  )
)