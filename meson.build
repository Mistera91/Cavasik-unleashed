project('cavasik', version: 'v2.0.2', meson_version: '>= 0.59.0', default_options: ['warning_level=2', 'werror=false'])

i18n = import('i18n')
gnome = import('gnome')

pkgdatadir = join_paths(get_option('prefix'), get_option('datadir'), meson.project_name())

subdir('assets')
subdir('src')
subdir('lang')

gnome.post_install(glib_compile_schemas: true, gtk_update_icon_cache: true, update_desktop_database: true)
