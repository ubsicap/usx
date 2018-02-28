.. include:: /_static/inc_styles.txt

.. index:: usx; attributes, attributes
.. _usx-attributes_index:
.. _usx-attributes_syntax:

Attributes
==========

Attributes are a standard aspect of XML syntax and can be applied to any element. An element can have multiple unique attributes. Attributes define additional properties of elements. They are a means of extending the meta information contained within in a USX text.

Attributes are listed as pairs of **name** and corresponding **value** using the syntax: ``attribute="value"``. The attribute name is a single ASCII string. The value is wrapped in quotes.

.. code-block:: xml

	<char style="w" lemma="grace">

Nearly all USX elements contain a required **@style** attribute. For :ref:`<para> <usx-element_para>` and :ref:`<char> <usx-element_char>` elements, the @style attribute defines the type of :doc:`paragraph <parastyles>` or :doc:`character <charstyles>` element being marked. The @style attribute in USX is also (intentionally) closely associated to `USFM <http://ubsicap.github.io/usfm/index.html>`_ paragraph and character markers with the same definition.

.. _usx-attributes_descriptive:
.. index:: attributes; descriptive

Word Level Descriptive Attributes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

|badge_3.0|

USX will formally provide additional descriptive attributes for a subset of :doc:`<char> @style types <charstyles>`. Each <char> element in this set will have a defined list of additional attribute(s), which are relevant to the overall purpose of the element.

.. _usx-attributes_default:

Default Attribute
^^^^^^^^^^^^^^^^^

The concept of a "default attribute" is only valid in USFM text. It was designed to reduce the amoung of metadata visible in the text when working with USFM. In the case of the `USFM specification <http://ubsicap.github.io/usfm/attributes/index.html>`_, a single default attribute may be defined for a given character marker, and does not require the attribute name to be written within the text. To be valid, the XML expression in USX must *always* contain the attribute name and its value.

In the preceding example, ``<char @style="w">`` accepts an additional attribute ``lemma``, which is the `default attribute <http://ubsicap.github.io/usfm/characters/index.html#usfmc-w-attr>`_ found in the USFM expression for the same text.

.. _usx-attributes_userDefined:

User Defined Attributes
^^^^^^^^^^^^^^^^^^^^^^^

User defined attributes may be added to any USX :ref:`<char> <usx-element_char>` element, even if it is not within the list of <char> @style type elements officially providing additional descriptive attributes. These will not be considered strictly USX compliant, and there is no assurance that they will be supported by compliant software tools or processes. Future versions of USX may formally define additional attributes.

Any user defined attributes must begin with the prefix ``x-``.

.. code-block:: xml

	<char style="w" x-myattr="metadata">gracious</char>
	<char style="w" lemma="grace" x-myattr="metadata">gracious</char>

.. _usx-attributes_styleTypesProviding:

<char> @style Types Providing Additional Attributes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* :ref:`<char @style="w"> <usx-charstyle_w-attr>` (lemma, strong, scrloc)

<ms> @style Types Providing Additional Attributes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* :ref:`<ms @style="qt#"> <usx-msstyle_qt-attr>` (who)