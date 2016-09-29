# Addons

`bl_info` is a dictionary containing addon meta-data such as the title, version and author to be displayed in the user preferences addon list.

	bl_info = {
		"category": "Object",
		"name": "My Test Addon"
	}

`register` is a function which only runs when enabling the addon.
This means the module can be loaded without activating the addon.

	def register():
		print("Hello World")

`unregister` is a function to unload anything setup by register.
This is called when the addon is disabled.

	def unregister():
		print("Goodbye World")

- https://www.blender.org/api/blender_python_api_current/info_tutorial_addon.html?highlight=register#what-is-an-addon