project('desktopicons-neo',
  version: '1.2',
  license: 'GPL3'
)

gnome = import ('gnome')
i18n = import('i18n')

prefix = get_option('prefix')
datadir = join_paths (prefix, get_option('datadir'))
schema_dir = join_paths(datadir, 'glib-2.0', 'schemas')

extensions_dir = join_paths(prefix, 'share', 'gnome-shell', 'extensions', 'desktopicons-neo@darkdemon')

install_data([
#    'createFolderDialog.js',
    'askConfirmPopup.js',
    'askNamePopup.js',
    'askRenamePopup.js',
    'createThumbnail.js',
    'dbusUtils.js',
    'desktopGrid.js',
    'desktopIconsUtil.js',
    'desktopManager.js',
    'desktopicons-neo.js',
    'emulateX11WindowType.js',
    'enums.js',
    'extension.js',
    'fileItem.js',
    'metadata.json',
    'prefs.js',
    'preferences.js',
    'showErrorPopup.js',
    'stylesheet.css',
    'templateManager.js'
  ],
  install_dir: extensions_dir
)

subdir(
  'po'
)
subdir(
  'schemas'
)

meson.add_install_script('meson_post_install.py')
