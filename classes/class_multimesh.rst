:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/MultiMesh.xml.

.. _class_MultiMesh:

MultiMesh
=========

**Inherits:** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Provides high-performance drawing of a mesh multiple times using GPU instancing.

Description
-----------

MultiMesh provides low-level mesh instancing. Drawing thousands of :ref:`MeshInstance3D<class_MeshInstance3D>` nodes can be slow, since each object is submitted to the GPU then drawn individually.

MultiMesh is much faster as it can draw thousands of instances with a single draw call, resulting in less API overhead.

As a drawback, if the instances are too far away from each other, performance may be reduced as every single instance will always render (they are spatially indexed as one, for the whole object).

Since instances may have any behavior, the AABB used for visibility must be provided by the user.

\ **Note:** A MultiMesh is a single object, therefore the same maximum lights per object restriction applies. This means, that once the maximum lights are consumed by one or more instances, the rest of the MultiMesh instances will **not** receive any lighting.

\ **Note:** Blend Shapes will be ignored if used in a MultiMesh.

Tutorials
---------

- :doc:`Animating thousands of fish with MultiMeshInstance <../tutorials/performance/vertex_animation/animating_thousands_of_fish>`

- :doc:`Optimization using MultiMeshes <../tutorials/performance/using_multimesh>`

Properties
----------

+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`PackedFloat32Array<class_PackedFloat32Array>`    | :ref:`buffer<class_MultiMesh_property_buffer>`                                 | ``PackedFloat32Array()`` |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`PackedColorArray<class_PackedColorArray>`        | :ref:`color_array<class_MultiMesh_property_color_array>`                       |                          |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`PackedColorArray<class_PackedColorArray>`        | :ref:`custom_data_array<class_MultiMesh_property_custom_data_array>`           |                          |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`int<class_int>`                                  | :ref:`instance_count<class_MultiMesh_property_instance_count>`                 | ``0``                    |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`Mesh<class_Mesh>`                                | :ref:`mesh<class_MultiMesh_property_mesh>`                                     |                          |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`PackedVector2Array<class_PackedVector2Array>`    | :ref:`transform_2d_array<class_MultiMesh_property_transform_2d_array>`         |                          |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`PackedVector3Array<class_PackedVector3Array>`    | :ref:`transform_array<class_MultiMesh_property_transform_array>`               |                          |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`TransformFormat<enum_MultiMesh_TransformFormat>` | :ref:`transform_format<class_MultiMesh_property_transform_format>`             | ``0``                    |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`bool<class_bool>`                                | :ref:`use_colors<class_MultiMesh_property_use_colors>`                         | ``false``                |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`bool<class_bool>`                                | :ref:`use_custom_data<class_MultiMesh_property_use_custom_data>`               | ``false``                |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+
| :ref:`int<class_int>`                                  | :ref:`visible_instance_count<class_MultiMesh_property_visible_instance_count>` | ``-1``                   |
+--------------------------------------------------------+--------------------------------------------------------------------------------+--------------------------+

Methods
-------

+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`               | :ref:`get_aabb<class_MultiMesh_method_get_aabb>` **(** **)** |const|                                                                                                           |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`             | :ref:`get_instance_color<class_MultiMesh_method_get_instance_color>` **(** :ref:`int<class_int>` instance **)** |const|                                                        |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`             | :ref:`get_instance_custom_data<class_MultiMesh_method_get_instance_custom_data>` **(** :ref:`int<class_int>` instance **)** |const|                                            |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Transform3D<class_Transform3D>` | :ref:`get_instance_transform<class_MultiMesh_method_get_instance_transform>` **(** :ref:`int<class_int>` instance **)** |const|                                                |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Transform2D<class_Transform2D>` | :ref:`get_instance_transform_2d<class_MultiMesh_method_get_instance_transform_2d>` **(** :ref:`int<class_int>` instance **)** |const|                                          |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_instance_color<class_MultiMesh_method_set_instance_color>` **(** :ref:`int<class_int>` instance, :ref:`Color<class_Color>` color **)**                               |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_instance_custom_data<class_MultiMesh_method_set_instance_custom_data>` **(** :ref:`int<class_int>` instance, :ref:`Color<class_Color>` custom_data **)**             |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_instance_transform<class_MultiMesh_method_set_instance_transform>` **(** :ref:`int<class_int>` instance, :ref:`Transform3D<class_Transform3D>` transform **)**       |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_instance_transform_2d<class_MultiMesh_method_set_instance_transform_2d>` **(** :ref:`int<class_int>` instance, :ref:`Transform2D<class_Transform2D>` transform **)** |
+---------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_MultiMesh_TransformFormat:

.. _class_MultiMesh_constant_TRANSFORM_2D:

.. _class_MultiMesh_constant_TRANSFORM_3D:

enum **TransformFormat**:

- **TRANSFORM_2D** = **0** --- Use this when using 2D transforms.

- **TRANSFORM_3D** = **1** --- Use this when using 3D transforms.

Property Descriptions
---------------------

.. _class_MultiMesh_property_buffer:

- :ref:`PackedFloat32Array<class_PackedFloat32Array>` **buffer**

+-----------+--------------------------+
| *Default* | ``PackedFloat32Array()`` |
+-----------+--------------------------+
| *Setter*  | set_buffer(value)        |
+-----------+--------------------------+
| *Getter*  | get_buffer()             |
+-----------+--------------------------+

----

.. _class_MultiMesh_property_color_array:

- :ref:`PackedColorArray<class_PackedColorArray>` **color_array**

See :ref:`set_instance_color<class_MultiMesh_method_set_instance_color>`.

----

.. _class_MultiMesh_property_custom_data_array:

- :ref:`PackedColorArray<class_PackedColorArray>` **custom_data_array**

See :ref:`set_instance_custom_data<class_MultiMesh_method_set_instance_custom_data>`.

----

.. _class_MultiMesh_property_instance_count:

- :ref:`int<class_int>` **instance_count**

+-----------+---------------------------+
| *Default* | ``0``                     |
+-----------+---------------------------+
| *Setter*  | set_instance_count(value) |
+-----------+---------------------------+
| *Getter*  | get_instance_count()      |
+-----------+---------------------------+

Number of instances that will get drawn. This clears and (re)sizes the buffers. Setting data format or flags afterwards will have no effect.

By default, all instances are drawn but you can limit this with :ref:`visible_instance_count<class_MultiMesh_property_visible_instance_count>`.

----

.. _class_MultiMesh_property_mesh:

- :ref:`Mesh<class_Mesh>` **mesh**

+----------+-----------------+
| *Setter* | set_mesh(value) |
+----------+-----------------+
| *Getter* | get_mesh()      |
+----------+-----------------+

:ref:`Mesh<class_Mesh>` resource to be instanced.

The looks of the individual instances can be modified using :ref:`set_instance_color<class_MultiMesh_method_set_instance_color>` and :ref:`set_instance_custom_data<class_MultiMesh_method_set_instance_custom_data>`.

----

.. _class_MultiMesh_property_transform_2d_array:

- :ref:`PackedVector2Array<class_PackedVector2Array>` **transform_2d_array**

See :ref:`set_instance_transform_2d<class_MultiMesh_method_set_instance_transform_2d>`.

----

.. _class_MultiMesh_property_transform_array:

- :ref:`PackedVector3Array<class_PackedVector3Array>` **transform_array**

See :ref:`set_instance_transform<class_MultiMesh_method_set_instance_transform>`.

----

.. _class_MultiMesh_property_transform_format:

- :ref:`TransformFormat<enum_MultiMesh_TransformFormat>` **transform_format**

+-----------+-----------------------------+
| *Default* | ``0``                       |
+-----------+-----------------------------+
| *Setter*  | set_transform_format(value) |
+-----------+-----------------------------+
| *Getter*  | get_transform_format()      |
+-----------+-----------------------------+

Format of transform used to transform mesh, either 2D or 3D.

----

.. _class_MultiMesh_property_use_colors:

- :ref:`bool<class_bool>` **use_colors**

+-----------+-----------------------+
| *Default* | ``false``             |
+-----------+-----------------------+
| *Setter*  | set_use_colors(value) |
+-----------+-----------------------+
| *Getter*  | is_using_colors()     |
+-----------+-----------------------+

If ``true``, the ``MultiMesh`` will use color data (see :ref:`set_instance_color<class_MultiMesh_method_set_instance_color>`). Can only be set when :ref:`instance_count<class_MultiMesh_property_instance_count>` is ``0`` or less. This means that you need to call this method before setting the instance count, or temporarily reset it to ``0``.

----

.. _class_MultiMesh_property_use_custom_data:

- :ref:`bool<class_bool>` **use_custom_data**

+-----------+----------------------------+
| *Default* | ``false``                  |
+-----------+----------------------------+
| *Setter*  | set_use_custom_data(value) |
+-----------+----------------------------+
| *Getter*  | is_using_custom_data()     |
+-----------+----------------------------+

If ``true``, the ``MultiMesh`` will use custom data (see :ref:`set_instance_custom_data<class_MultiMesh_method_set_instance_custom_data>`). Can only be set when :ref:`instance_count<class_MultiMesh_property_instance_count>` is ``0`` or less. This means that you need to call this method before setting the instance count, or temporarily reset it to ``0``.

----

.. _class_MultiMesh_property_visible_instance_count:

- :ref:`int<class_int>` **visible_instance_count**

+-----------+-----------------------------------+
| *Default* | ``-1``                            |
+-----------+-----------------------------------+
| *Setter*  | set_visible_instance_count(value) |
+-----------+-----------------------------------+
| *Getter*  | get_visible_instance_count()      |
+-----------+-----------------------------------+

Limits the number of instances drawn, -1 draws all instances. Changing this does not change the sizes of the buffers.

Method Descriptions
-------------------

.. _class_MultiMesh_method_get_aabb:

- :ref:`AABB<class_AABB>` **get_aabb** **(** **)** |const|

Returns the visibility axis-aligned bounding box in local space.

----

.. _class_MultiMesh_method_get_instance_color:

- :ref:`Color<class_Color>` **get_instance_color** **(** :ref:`int<class_int>` instance **)** |const|

Gets a specific instance's color multiplier.

----

.. _class_MultiMesh_method_get_instance_custom_data:

- :ref:`Color<class_Color>` **get_instance_custom_data** **(** :ref:`int<class_int>` instance **)** |const|

Returns the custom data that has been set for a specific instance.

----

.. _class_MultiMesh_method_get_instance_transform:

- :ref:`Transform3D<class_Transform3D>` **get_instance_transform** **(** :ref:`int<class_int>` instance **)** |const|

Returns the :ref:`Transform3D<class_Transform3D>` of a specific instance.

----

.. _class_MultiMesh_method_get_instance_transform_2d:

- :ref:`Transform2D<class_Transform2D>` **get_instance_transform_2d** **(** :ref:`int<class_int>` instance **)** |const|

Returns the :ref:`Transform2D<class_Transform2D>` of a specific instance.

----

.. _class_MultiMesh_method_set_instance_color:

- void **set_instance_color** **(** :ref:`int<class_int>` instance, :ref:`Color<class_Color>` color **)**

Sets the color of a specific instance by *multiplying* the mesh's existing vertex colors. This allows for different color tinting per instance.

For the color to take effect, ensure that :ref:`use_colors<class_MultiMesh_property_use_colors>` is ``true`` on the ``MultiMesh`` and :ref:`BaseMaterial3D.vertex_color_use_as_albedo<class_BaseMaterial3D_property_vertex_color_use_as_albedo>` is ``true`` on the material. If you intend to set an absolute color instead of tinting, make sure the material's albedo color is set to pure white (``Color(1, 1, 1)``).

----

.. _class_MultiMesh_method_set_instance_custom_data:

- void **set_instance_custom_data** **(** :ref:`int<class_int>` instance, :ref:`Color<class_Color>` custom_data **)**

Sets custom data for a specific instance. Although :ref:`Color<class_Color>` is used, it is just a container for 4 floating point numbers.

For the custom data to be used, ensure that :ref:`use_custom_data<class_MultiMesh_property_use_custom_data>` is ``true``.

This custom instance data has to be manually accessed in your custom shader using ``INSTANCE_CUSTOM``.

----

.. _class_MultiMesh_method_set_instance_transform:

- void **set_instance_transform** **(** :ref:`int<class_int>` instance, :ref:`Transform3D<class_Transform3D>` transform **)**

Sets the :ref:`Transform3D<class_Transform3D>` for a specific instance.

----

.. _class_MultiMesh_method_set_instance_transform_2d:

- void **set_instance_transform_2d** **(** :ref:`int<class_int>` instance, :ref:`Transform2D<class_Transform2D>` transform **)**

Sets the :ref:`Transform2D<class_Transform2D>` for a specific instance.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
