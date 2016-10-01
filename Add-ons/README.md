# Add-ons

`bl_info` is a Dictionary containing add-on meta-data such as the `author`, `name`, and `version` to be displayed in the user preferences add-on list.

	bl_info = {
		'author': 'Matt McKellar-Spence',
		'blender': (2, 75, 0),
		'category': 'Object',
		'description': 'Adds a new Mesh Object',
		'location': 'View3D > Add > Mesh > New Object',
		'name': 'My Test Addon'
		'warning': '',
		'wiki_url': '',
		'version': (1, 0),
	}

`register` is a function which only runs when enabling the add-on.
This means the module can be loaded without activating the add-on.

	def register():
		print('Hello World')

`unregister` is a function to unload anything setup by `register`.
This is called when the add-on is disabled.

	def unregister():
		print('Goodbye World')


## Reference

- [What is an Addon? @ Current API](https://www.blender.org/api/blender_python_api_current/info_tutorial_addon.html#what-is-an-addon)
