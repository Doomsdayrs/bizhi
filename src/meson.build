bizhi_sources = [
  'main.cpp',
  'bizhi-window.cpp',
]

bizhi_deps = [
  dependency('gtkmm-3.0', version: '>= 3.18'),
]

gnome = import('gnome')

bizhi_sources += gnome.compile_resources('bizhi-resources',
  'bizhi.gresource.xml',
  c_name: 'bizhi'
)

executable('bizhi', bizhi_sources,
  dependencies: bizhi_deps,
  install: true,
)
