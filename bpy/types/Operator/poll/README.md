# bpy.types.Operator.poll

Return `True` if the Operator can be run.

- [bpy.types.Operator.poll @ Current API](https://www.blender.org/api/blender_python_api_current/bpy.types.Operator.html#bpy.types.Operator.poll)

```
class MyOperator(bpy.types.Operator):

	@classmethod
	def poll(cls, context):
		return context.object is not None
```
