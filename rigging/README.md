# Rigging

- [Rigging @ Blender manual](https://www.blender.org/manual/rigging/index.html)

You define a "Rest" position of Bones before their "Pose" position.
Later, if you update the Rest position then Poses will update too.


## Bone names

"Head" or "Root"
: Ball at the wide end of the Bone.
: Root is the preferred name.

"Tail" or "Tip"
: Ball at the narrow end of the Bone.
: Tip is the preferred name.

"Body"
: Main part of the Bone.

- https://www.blender.org/manual/en/rigging/armatures/bones/introduction.html
- https://wiki.blender.org/index.php/Doc:2.4/Manual/Rigging/Armatures/Bones


## Adding Bones

1. `Shift + a` to open the "Add" menu; under "Armature" click "Single Bone".

2. `Tab` to enter "Edit Mode".

3. Right-click the Tail; type `e` to extrude a linked Bone.
Extruding from the Head will create an unlinked Bone, with its Head at the same place.


## Skinning

- [Skinning @ Blender manual](https://www.blender.org/manual/rigging/skinning.html)

1. Select something in Object Mode.

2. In the "Properties" Panel click "Constraints".

3. Click "Add Object Constraint", then under "Relationship" click "Child Of".

4. For "Target" select your Armature Object.

The original Object will now follow your movements of the Armature.
