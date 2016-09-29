# bpy.context.copy

Get a copy of the Context that can then be modified.

This is useful for passing in a different Context to Operators.

```
# Remove all objects in Scene rather than the selected ones.
import bpy
override = bpy.context.copy()
override['selected_bases'] = list(bpy.context.scene.object_bases)
bpy.ops.object.delete(override)
```

- [Overriding Context @ Current API](https://www.blender.org/api/blender_python_api_current/bpy.ops.html#overriding-context)
