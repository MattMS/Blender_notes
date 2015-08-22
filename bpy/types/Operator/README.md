# Operator

- [Operator @ API 2.74](http://www.blender.org/api/blender_python_api_2_74_release/bpy.types.Operator.html)

```python
import bpy

class MyOperator(bpy.types.Operator):
	bl_idname = 'wm.my_op'
	bl_label = 'My Operator'

	x = bpy.props.IntProperty()
	y = bpy.props.IntProperty()

	def execute(self, context):
		print('Done')
		return {'FINISHED'}

	def invoke(self, context, event):
		self.x = event.mouse_x
		self.y = event.mouse_y
		return self.execute(context)

bpy.utils.register_class(MyOperator)
```
