:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/modules/openxr/doc_classes/OpenXRInterface.xml.

.. _class_OpenXRInterface:

OpenXRInterface
===============

**Inherits:** :ref:`XRInterface<class_XRInterface>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Our OpenXR interface.

Description
-----------

The OpenXR interface allows Godot to interact with OpenXR runtimes and make it possible to create XR experiences and games.

Due to the needs of OpenXR this interface works slightly different than other plugin based XR interfaces. It needs to be initialized when Godot starts. You need to enable OpenXR, settings for this can be found in your games project settings under the XR heading. You do need to mark a viewport for use with XR in order for Godot to know which render result should be output to the headset.

Tutorials
---------

- :doc:`Setting up XR <../tutorials/xr/setting_up_xr>`

Properties
----------

+---------------------------+----------------------------------------------------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`display_refresh_rate<class_OpenXRInterface_property_display_refresh_rate>` | ``0.0`` |
+---------------------------+----------------------------------------------------------------------------------+---------+

Methods
-------

+---------------------------+----------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>` | :ref:`get_available_display_refresh_rates<class_OpenXRInterface_method_get_available_display_refresh_rates>` **(** **)** |const| |
+---------------------------+----------------------------------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_OpenXRInterface_signal_pose_recentered:

- **pose_recentered** **(** **)**

Informs the user queued a recenter of the player position.

----

.. _class_OpenXRInterface_signal_session_begun:

- **session_begun** **(** **)**

Informs our OpenXR session has been started.

----

.. _class_OpenXRInterface_signal_session_focussed:

- **session_focussed** **(** **)**

Informs our OpenXR session now has focus.

----

.. _class_OpenXRInterface_signal_session_stopping:

- **session_stopping** **(** **)**

Informs our OpenXR session is stopping.

----

.. _class_OpenXRInterface_signal_session_visible:

- **session_visible** **(** **)**

Informs our OpenXR session is now visible (output is being sent to the HMD).

Property Descriptions
---------------------

.. _class_OpenXRInterface_property_display_refresh_rate:

- :ref:`float<class_float>` **display_refresh_rate**

+-----------+---------------------------------+
| *Default* | ``0.0``                         |
+-----------+---------------------------------+
| *Setter*  | set_display_refresh_rate(value) |
+-----------+---------------------------------+
| *Getter*  | get_display_refresh_rate()      |
+-----------+---------------------------------+

The display refresh rate for the current HMD. Only functional if this feature is supported by the OpenXR runtime and after the interface has been initialized.

Method Descriptions
-------------------

.. _class_OpenXRInterface_method_get_available_display_refresh_rates:

- :ref:`Array<class_Array>` **get_available_display_refresh_rates** **(** **)** |const|

Returns display refresh rates supported by the current HMD. Only returned if this feature is supported by the OpenXR runtime and after the interface has been initialized.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
