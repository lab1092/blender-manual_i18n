
..    TODO/Review: {{review|}} .

******
Mirror
******

.. admonition:: Reference
   :class: refbox

   | Mode:     *Edit* mode
   | Menu:     :menuselection:`Mesh --> Mirror --> Desired Axis`
   | Hotkey:   :kbd:`Ctrl-M`


The mirror tool mirrors a selection across a selected axis.

The mirror tool in *Edit* mode is similar to
:doc:`Mirroring in Object mode </modeling/meshes/editing/duplicating/mirror>`.
It is exactly equivalent to scaling by -1 vertices,
edges or faces around one chosen pivot point and in the direction of one chosen axis, only it is faster/handier.


After this tool becomes active, select an axis to mirror the selection on entering x,y, or z.

You can also interactively mirror the geometry by holding the :kbd:`MMB` and dragging in
the direction of the desired mirror direction.


Axis of symmetry
================

For each transformation orientation,
you can choose one of its axes along which the mirroring will occur.

As you can see, the possibilities are infinite and the freedom complete:
you can position the pivot point at any location around which we want the mirroring to occur,
choose one transformation orientation and then one axis on it.


Pivot point
===========

:doc:`Pivot points </editors/3dview/transform/transform_control/pivot_point/index>` must be set first.
Pivot points will become the center of symmetry.
If the widget is turned on it will always show where the pivot point is.


On (*Mirror around the Individual Centers ...*) the pivot point default to
**median point of the selection of vertices** in *Edit* mode.
This is a special case of the *Edit* mode as explained on the
:doc:`pivot point page </editors/3dview/transform/transform_control/pivot_point/index>`.


.. figure:: /images/MirrorTool1.jpg
   :width: 300px

   Mesh before mirror.


.. figure:: /images/MirrorTool2.jpg
   :width: 300px

   Mesh after mirrored along X axis


On (*Mirror around the 3D Cursor ...*)
the pivot point is the *3D Cursor*,
the transformation orientation is *Local*, a.k.a. the Object space,
and the axis of transformation is X.


.. figure:: /images/MirrorTool3.jpg
   :width: 300px

   Mesh before mirror.


.. figure:: /images/MirrorTool4.jpg
   :width: 300px

   Mesh after mirrored along X axis using the 3d cursor as a pivot point


Transformation orientation
==========================

:doc:`Transformation Orientations </editors/3dview/transform/transform_control/transform_orientations>`
are found on the 3D area header, next to the *Widget* buttons.
They decide which coordinate system will rule the mirroring.
