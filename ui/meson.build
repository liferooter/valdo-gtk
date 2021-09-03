gnome = import('gnome')

resources_xml = files('valdo-gtk.gresource.xml')
resources = gnome.compile_resources('resources', resources_xml, source_dir: '.')

resource_args = [ # valac args
  '--gresources', resources_xml,
  '--target-glib=2.68' # minimum glib version required for composite templates
]
