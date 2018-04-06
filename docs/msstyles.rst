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
		who questioned him. <ms style="qt1-s" sid="qt1_MAT_27:11_a" who="Pilate"/>“Are you the 
		king of the Jews?”<ms style="qt1-e" eid="qt1_MAT_27:11_a"/> he asked.</para>
	<para style="p"><ms style="qt1-s" sid="qt1_MAT_27:11_b" who="Jesus"/>“So you say,”
		<ms style="qt1-e" eid="qt1_MAT_27:11_b"/> answered Jesus.
		<verse number="12" style="v"/>But he said nothing in response to the accusations of 
		the chief priests and elders.</para>
	<para style="p"><verse number="13" style="v"/>So Pilate said to him,
		<ms style="qt1-s" sid="qt1_MAT_27:13_a" who="Pilate"/>“Don't you hear all these things 
		they accuse you of?”<ms style="qt1-e" eid="qt1_MAT_27:13_a"/></para>
	<para style="p"><verse number="14" style="v"/>But Jesus refused to answer a single word, 
		with the result that the Governor was greatly surprised.</para>

-----

.. index:: ms@style; ts, milestones; translator's section
.. _usx-msstyle_ts:

ts
^^

|badge_3.0|

:@style: ts
:Use: Translator's section. |br|
    For identifying a section (chunk) of text suitable for translating at one time.
:Valid In: Any valid :ref:`usx-element_ms`

**Text Samples** - Jude 5-8, ULB - using standalone milestones

.. code-block:: xml
	:name: usx-msstyle_ts_example
	:emphasize-lines: 1,9,17

	<ms style="ts" />
	<para style="p">
		<verse number="5" style="v" />Now I wish to remind you, although you know everything, 
		that the Lord once saved a people out of the land of Egypt, but that afterward he 
		destroyed those who did not believe.
		<verse number="6" style="v" /> And angels who did not keep to their own principality, 
		but left their proper dwelling place—God has kept them in everlasting chains in 
		darkness for the judgment of the great day.
	<ms style="ts" />
		<verse number="7" style="v" />It is just like Sodom and Gomorrah and the cities 
		around them, which in a similar way gave themselves over to fornication and pursued 
		unnatural desires. They were given as examples of those who suffer the punishment of 
		eternal fire.
		<verse number="8" style="v" />Yet in the same way these also pollute their bodies in 
		their dreams, and they reject authority, and they say evil things about the glorious ones.
	</para>
	<ms style="ts" />

Jude 5-8, ULB - using milestone pairs

.. code-block:: xml
	:name: usx-msstyle_ts_example-alt
	:emphasize-lines: 1,9,10,18

	<ms style="ts-s" sid="ts_JUD_5-6" />
	<para style="p">
		<verse number="5" style="v" />Now I wish to remind you, although you know everything, 
		that the Lord once saved a people out of the land of Egypt, but that afterward he 
		destroyed those who did not believe.
		<verse number="6" style="v" /> And angels who did not keep to their own principality, 
		but left their proper dwelling place—God has kept them in everlasting chains in 
		darkness for the judgment of the great day.
	<ms style="ts-e" eid="ts_JUD_5-6" />
	<ms style="ts-s" sid="ts_JUD_7-8" />
		<verse number="7" style="v" />It is just like Sodom and Gomorrah and the cities 
		around them, which in a similar way gave themselves over to fornication and pursued 
		unnatural desires. They were given as examples of those who suffer the punishment of 
		eternal fire.
		<verse number="8" style="v" />Yet in the same way these also pollute their bodies in 
		their dreams, and they reject authority, and they say evil things about the glorious ones.
	</para>
	<ms style="ts-e" eid="ts_JUD_7-8" />