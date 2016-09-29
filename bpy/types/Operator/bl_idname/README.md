# bpy.types.Operator.bl_idname

Set the path under `bpy.ops` where this Operator is registered.

- [bl_idname @ API](https://www.blender.org/api/blender_python_api_current/bpy.types.Operator.html#bpy.types.Operator.bl_idname)

```
class MyOperator(bpy.types.Operator):

	bl_idname = 'object.modal_operator'

bpy.utils.register_class(MyOperator)

bpy.ops.object.modal_operator('INVOKE_DEFAULT')
```
