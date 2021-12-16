project('coreutils', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])

libuv_dep = dependency('libuv', fallback: ['libuv', 'libuv_dep'])
uvcat = executable('uvcat', 'src/uvcat.c',
  dependencies : libuv_dep,
  install : true)

test('uvcat', uvcat)
