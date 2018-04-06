.. include:: /_static/inc_styles.txt

.. index:: attribute; ms@style, milestones
.. _usx-msstyles:

<ms> @style Types
=================

.. _usx-notes_numberedStyles-ms:

.. note:: **Numbered <ms> @style Attributes**

    As with USX :ref:`<para> <usx-element_para>` elements which include a numeric variable in the @style attribute, a number may be added to a milestone @style attribute to indicate a relative weighting or level.
    
    **style = style1** — The unnumbered version of a style attribute may be used when only one level of this milestone style exists within the project text. Numbers should always be included when more than one level of the milestone style exists within the project text.

-----

.. index:: ms@style; qt, milestones; quotations
.. _usx-msstyle_qt:

qt#
^^^

|badge_3.0|

:@style: qt#
:Use: Quotation speaker. |br|
    # denotes the level of nesting of the quotation being marked (i.e. a quote within a quote). |br|
    **qt = qt1** (see :ref:`notes <usx-notes_numberedStyles-ms>` on numbered @style attributes)
:Valid In: Any valid :ref:`usx-element_ms`

.. _usx-msstyle_qt-attr:
.. index:: attribute; ms@who (@style="qt#"), quotation speaker; attributes

.. rubric:: Attributes |ico_Tag|

*Additional* :doc:`attributes <attributes>` for :ref:`<ms> <usx-element_ms>` which can be used in this context.

:@who: The speaker of the current quotation.

.. code-block:: xml

    <ms style="qt1-s" who="Paul"/>

**Text Samples** - Matthew 27.11-14 (GNT)

.. code-block:: xml
	:name: usx-msstyle_qt_example
	
	<para style="p"><verse number="11" style="v">Jesus stood before the Roman governor, 
		who questioned him. <ms style="qt1-s" sid="MAT.27.11.a" who="Pilate"/>“Are you the 
		king of the Jews?”<ms style="qt1-e" eid="MAT.27.11.a"/> he asked.</para>
	<para style="p"><ms style="qt1-s" sid="MAT.27.11.b" who="Jesus"/>“So you say,”
		<ms style="qt1-e" eid="MAT.27.11.1b"/> answered Jesus.
		<verse number="12" style="v"/>But he said nothing in response to the accusations of 
		the chief priests and elders.</para>
	<para style="p"><verse number="13" style="v"/>So Pilate said to him,
		<ms style="qt1-s" sid="MAT.27.13.a" who="Pilate"/>“Don't you hear all these things 
		they accuse you of?”<ms style="qt1-e" eid="MAT.27.13.a"/></para>
	<para style="p"><verse number="14" style="v"/>But Jesus refused to answer a single word, 
		with the result that the Governor was greatly surprised.</para>
