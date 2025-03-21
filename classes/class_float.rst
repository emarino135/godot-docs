:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/float.xml.

.. _class_float:

float
=====

Float built-in type.

Description
-----------

The ``float`` built-in type is a 64-bit double-precision floating-point number, equivalent to ``double`` in C++. This type has 14 reliable decimal digits of precision. The ``float`` type can be stored in :ref:`Variant<class_Variant>`, which is the generic type used by the engine. The maximum value of ``float`` is approximately ``1.79769e308``, and the minimum is approximately ``-1.79769e308``.

Many methods and properties in the engine use 32-bit single-precision floating-point numbers instead, equivalent to ``float`` in C++, which have 6 reliable decimal digits of precision. For data structures such as :ref:`Vector2<class_Vector2>` and :ref:`Vector3<class_Vector3>`, Godot uses 32-bit floating-point numbers by default, but it can be changed to use 64-bit doubles if Godot is compiled with the ``float=64`` option.

Math done using the ``float`` type is not guaranteed to be exact or deterministic, and will often result in small errors. You should usually use the :ref:`@GlobalScope.is_equal_approx<class_@GlobalScope_method_is_equal_approx>` and :ref:`@GlobalScope.is_zero_approx<class_@GlobalScope_method_is_zero_approx>` methods instead of ``==`` to compare ``float`` values for equality.

Tutorials
---------

- `Wikipedia: Double-precision floating-point format <https://en.wikipedia.org/wiki/Double-precision_floating-point_format>`__

- `Wikipedia: Single-precision floating-point format <https://en.wikipedia.org/wiki/Single-precision_floating-point_format>`__

Constructors
------------

+---------------------------+----------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>` **(** **)**                                |
+---------------------------+----------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>` **(** :ref:`float<class_float>` from **)** |
+---------------------------+----------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>` **(** :ref:`bool<class_bool>` from **)**   |
+---------------------------+----------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`float<class_float_constructor_float>` **(** :ref:`int<class_int>` from **)**     |
+---------------------------+----------------------------------------------------------------------------------------+

Operators
---------

+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator !=<class_float_operator_neq_bool>` **(** :ref:`float<class_float>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator !=<class_float_operator_neq_bool>` **(** :ref:`int<class_int>` right **)**                    |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`           | :ref:`operator *<class_float_operator_mul_Color>` **(** :ref:`Color<class_Color>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Quaternion<class_Quaternion>` | :ref:`operator *<class_float_operator_mul_Quaternion>` **(** :ref:`Quaternion<class_Quaternion>` right **)** |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`       | :ref:`operator *<class_float_operator_mul_Vector2>` **(** :ref:`Vector2<class_Vector2>` right **)**          |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`       | :ref:`operator *<class_float_operator_mul_Vector2>` **(** :ref:`Vector2i<class_Vector2i>` right **)**        |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`       | :ref:`operator *<class_float_operator_mul_Vector3>` **(** :ref:`Vector3<class_Vector3>` right **)**          |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`       | :ref:`operator *<class_float_operator_mul_Vector3>` **(** :ref:`Vector3i<class_Vector3i>` right **)**        |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Vector4<class_Vector4>`       | :ref:`operator *<class_float_operator_mul_Vector4>` **(** :ref:`Vector4<class_Vector4>` right **)**          |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`Vector4<class_Vector4>`       | :ref:`operator *<class_float_operator_mul_Vector4>` **(** :ref:`Vector4i<class_Vector4i>` right **)**        |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator *<class_float_operator_mul_float>` **(** :ref:`float<class_float>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator *<class_float_operator_mul_float>` **(** :ref:`int<class_int>` right **)**                    |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator **<class_float_operator_pow_float>` **(** :ref:`float<class_float>` right **)**               |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator **<class_float_operator_pow_float>` **(** :ref:`int<class_int>` right **)**                   |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator +<class_float_operator_sum_float>` **(** :ref:`float<class_float>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator +<class_float_operator_sum_float>` **(** :ref:`int<class_int>` right **)**                    |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator -<class_float_operator_dif_float>` **(** :ref:`float<class_float>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator -<class_float_operator_dif_float>` **(** :ref:`int<class_int>` right **)**                    |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator /<class_float_operator_div_float>` **(** :ref:`float<class_float>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator /<class_float_operator_div_float>` **(** :ref:`int<class_int>` right **)**                    |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator \<<class_float_operator_lt_bool>` **(** :ref:`float<class_float>` right **)**                 |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator \<<class_float_operator_lt_bool>` **(** :ref:`int<class_int>` right **)**                     |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator \<=<class_float_operator_lte_bool>` **(** :ref:`float<class_float>` right **)**               |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator \<=<class_float_operator_lte_bool>` **(** :ref:`int<class_int>` right **)**                   |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator ==<class_float_operator_eq_bool>` **(** :ref:`float<class_float>` right **)**                 |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator ==<class_float_operator_eq_bool>` **(** :ref:`int<class_int>` right **)**                     |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator ><class_float_operator_gt_bool>` **(** :ref:`float<class_float>` right **)**                  |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator ><class_float_operator_gt_bool>` **(** :ref:`int<class_int>` right **)**                      |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator >=<class_float_operator_gte_bool>` **(** :ref:`float<class_float>` right **)**                |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`operator >=<class_float_operator_gte_bool>` **(** :ref:`int<class_int>` right **)**                    |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator unary+<class_float_operator_unplus_float>` **(** **)**                                        |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`           | :ref:`operator unary-<class_float_operator_unminus_float>` **(** **)**                                       |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------+

Constructor Descriptions
------------------------

.. _class_float_constructor_float:

- :ref:`float<class_float>` **float** **(** **)**

Constructs a default-initialized ``float`` set to ``0.0``.

----

- :ref:`float<class_float>` **float** **(** :ref:`float<class_float>` from **)**

Constructs a ``float`` as a copy of the given ``float``.

----

- :ref:`float<class_float>` **float** **(** :ref:`bool<class_bool>` from **)**

Cast a :ref:`bool<class_bool>` value to a floating-point value, ``float(true)`` will be equal to 1.0 and ``float(false)`` will be equal to 0.0.

----

- :ref:`float<class_float>` **float** **(** :ref:`int<class_int>` from **)**

Cast an :ref:`int<class_int>` value to a floating-point value, ``float(1)`` will be equal to ``1.0``.

Operator Descriptions
---------------------

.. _class_float_operator_neq_bool:

- :ref:`bool<class_bool>` **operator !=** **(** :ref:`float<class_float>` right **)**

Returns ``true`` if two floats are different from each other.

----

- :ref:`bool<class_bool>` **operator !=** **(** :ref:`int<class_int>` right **)**

Returns ``true`` if the integer has different value than the float.

----

.. _class_float_operator_mul_Color:

- :ref:`Color<class_Color>` **operator *** **(** :ref:`Color<class_Color>` right **)**

Multiplies each component of the :ref:`Color<class_Color>` by the given ``float``.

::

    print(1.5 * Color(0.5, 0.5, 0.5)) # Color(0.75, 0.75, 0.75)

----

- :ref:`Quaternion<class_Quaternion>` **operator *** **(** :ref:`Quaternion<class_Quaternion>` right **)**

Multiplies each component of the :ref:`Quaternion<class_Quaternion>` by the given ``float``. This operation is not meaningful on its own, but it can be used as a part of a larger expression.

----

- :ref:`Vector2<class_Vector2>` **operator *** **(** :ref:`Vector2<class_Vector2>` right **)**

Multiplies each component of the :ref:`Vector2<class_Vector2>` by the given ``float``.

::

    print(2.5 * Vector2(1, 3)) # Prints "(2.5, 7.5)"

----

- :ref:`Vector2<class_Vector2>` **operator *** **(** :ref:`Vector2i<class_Vector2i>` right **)**

Multiplies each component of the :ref:`Vector2i<class_Vector2i>` by the given ``float``. Returns a :ref:`Vector2<class_Vector2>`.

::

    print(0.9 * Vector2i(10, 15)) # Prints "(9, 13.5)"

----

- :ref:`Vector3<class_Vector3>` **operator *** **(** :ref:`Vector3<class_Vector3>` right **)**

Multiplies each component of the :ref:`Vector3<class_Vector3>` by the given ``float``.

----

- :ref:`Vector3<class_Vector3>` **operator *** **(** :ref:`Vector3i<class_Vector3i>` right **)**

Multiplies each component of the :ref:`Vector3i<class_Vector3i>` by the given ``float``. Returns a :ref:`Vector3<class_Vector3>`.

::

    print(0.9 * Vector3i(10, 15, 20)) # Prints "(9, 13.5, 18)"

----

- :ref:`Vector4<class_Vector4>` **operator *** **(** :ref:`Vector4<class_Vector4>` right **)**

Multiplies each component of the :ref:`Vector4<class_Vector4>` by the given ``float``.

----

- :ref:`Vector4<class_Vector4>` **operator *** **(** :ref:`Vector4i<class_Vector4i>` right **)**

Multiplies each component of the :ref:`Vector4i<class_Vector4i>` by the given ``float``. Returns a :ref:`Vector4<class_Vector4>`.

::

    print(0.9 * Vector4i(10, 15, 20, -10)) # Prints "(9, 13.5, 18, -9)"

----

- :ref:`float<class_float>` **operator *** **(** :ref:`float<class_float>` right **)**

Multiplies two ``float``\ s.

----

- :ref:`float<class_float>` **operator *** **(** :ref:`int<class_int>` right **)**

Multiplies a ``float`` and an :ref:`int<class_int>`. The result is a ``float``.

----

.. _class_float_operator_pow_float:

- :ref:`float<class_float>` **operator **** **(** :ref:`float<class_float>` right **)**

Raises a ``float`` to a power of a ``float``.

::

    print(39.0625**0.25) # 2.5

----

- :ref:`float<class_float>` **operator **** **(** :ref:`int<class_int>` right **)**

Raises a ``float`` to a power of an :ref:`int<class_int>`. The result is a ``float``.

::

    print(0.9**3) # 0.729

----

.. _class_float_operator_sum_float:

- :ref:`float<class_float>` **operator +** **(** :ref:`float<class_float>` right **)**

Adds two floats.

----

- :ref:`float<class_float>` **operator +** **(** :ref:`int<class_int>` right **)**

Adds a ``float`` and an :ref:`int<class_int>`. The result is a ``float``.

----

.. _class_float_operator_dif_float:

- :ref:`float<class_float>` **operator -** **(** :ref:`float<class_float>` right **)**

Subtracts a float from a float.

----

- :ref:`float<class_float>` **operator -** **(** :ref:`int<class_int>` right **)**

Subtracts an :ref:`int<class_int>` from a ``float``. The result is a ``float``.

----

.. _class_float_operator_div_float:

- :ref:`float<class_float>` **operator /** **(** :ref:`float<class_float>` right **)**

Divides two floats.

----

- :ref:`float<class_float>` **operator /** **(** :ref:`int<class_int>` right **)**

Divides a ``float`` by an :ref:`int<class_int>`. The result is a ``float``.

----

.. _class_float_operator_lt_bool:

- :ref:`bool<class_bool>` **operator <** **(** :ref:`float<class_float>` right **)**

Returns ``true`` if the left float is less than the right one.

----

- :ref:`bool<class_bool>` **operator <** **(** :ref:`int<class_int>` right **)**

Returns ``true`` if this ``float`` is less than the given :ref:`int<class_int>`.

----

.. _class_float_operator_lte_bool:

- :ref:`bool<class_bool>` **operator <=** **(** :ref:`float<class_float>` right **)**

Returns ``true`` if the left float is less than or equal to the right one.

----

- :ref:`bool<class_bool>` **operator <=** **(** :ref:`int<class_int>` right **)**

Returns ``true`` if this ``float`` is less than or equal to the given :ref:`int<class_int>`.

----

.. _class_float_operator_eq_bool:

- :ref:`bool<class_bool>` **operator ==** **(** :ref:`float<class_float>` right **)**

Returns ``true`` if both floats are exactly equal.

\ **Note:** Due to floating-point precision errors, consider using :ref:`@GlobalScope.is_equal_approx<class_@GlobalScope_method_is_equal_approx>` or :ref:`@GlobalScope.is_zero_approx<class_@GlobalScope_method_is_zero_approx>` instead, which are more reliable.

----

- :ref:`bool<class_bool>` **operator ==** **(** :ref:`int<class_int>` right **)**

Returns ``true`` if the ``float`` and the given :ref:`int<class_int>` are equal.

----

.. _class_float_operator_gt_bool:

- :ref:`bool<class_bool>` **operator >** **(** :ref:`float<class_float>` right **)**

Returns ``true`` if the left float is greater than the right one.

----

- :ref:`bool<class_bool>` **operator >** **(** :ref:`int<class_int>` right **)**

Returns ``true`` if this ``float`` is greater than the given :ref:`int<class_int>`.

----

.. _class_float_operator_gte_bool:

- :ref:`bool<class_bool>` **operator >=** **(** :ref:`float<class_float>` right **)**

Returns ``true`` if the left float is greater than or equal to the right one.

----

- :ref:`bool<class_bool>` **operator >=** **(** :ref:`int<class_int>` right **)**

Returns ``true`` if this ``float`` is greater than or equal to the given :ref:`int<class_int>`.

----

.. _class_float_operator_unplus_float:

- :ref:`float<class_float>` **operator unary+** **(** **)**

Returns the same value as if the ``+`` was not there. Unary ``+`` does nothing, but sometimes it can make your code more readable.

----

.. _class_float_operator_unminus_float:

- :ref:`float<class_float>` **operator unary-** **(** **)**

Returns the negative value of the ``float``. If positive, turns the number negative. If negative, turns the number positive. With floats, the number zero can be either positive or negative.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
