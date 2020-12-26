project(
  'com.paysonwallach.zeitgeist.bridge',
  'vala',
  'c',
  license: 'GPL-3.0',
  meson_version: '>=0.55.0',
  version: '0.1.0'
)

pymod = import('python')

python = pymod.find_installation('python3')

sources = files('src/gnome_dictionary_lookup.py')

python.install_sources(sources)

meson.add_install_script(
  'meson/post_install.py',
  get_option('browsers')
)
