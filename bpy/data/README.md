# bpy.data

## Create object

Objects cannot be created directly from classes.
They must be created through collections.

	>>> mesh = bpy.data.meshes.new(name="MyMesh")
	>>> print(mesh)
	<bpy_struct, Mesh("MyMesh.001")>
