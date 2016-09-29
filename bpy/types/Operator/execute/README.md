# bpy.types.Operator.execute

- [execute(context) @ API](https://www.blender.org/api/blender_python_api_current/bpy.types.Operator.html#bpy.types.Operator.execute)

Operators without `execute()` do not have the ability to be repeated from a script or macro.


```
class MyOperator(bpy.types.Operator):

	bl_idname = 'wm.mouse_position'
	bl_label = 'Invoke Mouse Operator'

	x = bpy.props.IntProperty()

	def execute(self, context):
		return {'FINISHED'}

bpy.utils.register_class(MyOperator)

bpy.ops.wm.mouse_position('INVOKE_DEFAULT')

bpy.ops.wm.mouse_position('EXEC_DEFAULT', x=12)
```


## Return value

CANCELLED
: When no action has been taken, operator exits.

FINISHED
: When the operator is complete, operator exits.

INTERFACE
: Handled but not executed (popup menus).

PASS_THROUGH
: Do nothing and pass the event on.

RUNNING_MODAL
: Keep the operator running with blender.
