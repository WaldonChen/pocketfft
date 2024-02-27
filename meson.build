project('pocketfft', 'cpp', version: '0.1.0',
  default_options : ['cpp_std=c++11'])

install_headers(files('pocketfft_hdronly.h'))

pkgc = import('pkgconfig')

pkgc.generate(name: 'pocketfft',
  version: meson.project_version(),
  subdirs: 'pocketfft',
  description: 'PocketFFT for C++'
)

pocketfft_dep = declare_dependency(
  include_directories: include_directories('.')
)
