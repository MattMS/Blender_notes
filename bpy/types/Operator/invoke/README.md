# bpy.types.Operator.invoke

Usually used to assign [properties](/bpy/props) from context when Operator is called.

- [invoke @ API](https://www.blender.org/api/blender_python_api_current/bpy.types.Operator.html#invoke-function)

```
class MyOperator(bpy.types.Operator):
	x = bpy.props.IntProperty()

	def invoke(self, context, event):
		self.x = event.mouse_x
		return self.execute(context)
```
