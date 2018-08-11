.. include:: /_static/inc_styles.txt

.. _usx-note:

<note> Types
============

.. contents::
	:depth: 2

-----

.. index:: usx <note> (footnote)
.. index:: usx <note> (endnote)
.. index:: usx <note> (study note)
.. _usx-note_footnote:

<note> (Footnote)
-----------------
|ico_R| Schema pattern name: **Footnote**

:Element: note |br|
	*empty* (all content is contained within the note's child char elements)
:Added: 1.0
:Use: Contains child :ref:`usx-element_char` elements to contain the content for a footnote, endnote, or study note.
:@caller: Note caller. |req| |br|
	``+`` | ``-`` | <user defined caller> |br|
	*A <user defined caller> may be any single character or sequence of characters preferred as the caller for a note.*
:@style: Content (footnote) type. |req| |br|
	``f`` (footnote) | ``fe`` (endnote) | ``ef`` (extended / study note)
:Valid in: :ref:`usx-div_bookTitles`, :ref:`usx-div_bookIntroduction`, :ref:`usx-div_introductionEndTitles`, :ref:`usx-div_chapterText`
:Parents: :ref:`usx-element_para`, :ref:`usx-element_char`, :ref:`usx-element_cell`

Diagram
"""""""

.. image:: images/usx-pattern_Footnote.png

.. index:: usx <char> (footnote)
.. _usx-note_footnote_char:

<char> (Footnote)
^^^^^^^^^^^^^^^^^
|ico_R| Schema pattern name: **FootnoteChar**

:Element: char |br|
	xsd:string
:Added: 1.0
:Use: An element for marking various footnote content types.
:@style: Footnote content type. |req| |br|
	The :ref:`usx-element_char` (Footnote) @style types list (below) presents an itemization of @style values valid within :ref:`usx-element_char` elements which are children of :ref:`usx-element_note` @style="f", :ref:`usx-element_note` @style="fe", and :ref:`usx-element_note` @style="ef".
:Valid in: :ref:`usx-note_footnote`

Diagram
"""""""

.. image:: images/usx-pattern_FootnoteChar.png

.. _usx-note_footnote_charstyles:

<char> (Footnote) @style Types
""""""""""""""""""""""""""""""

* :ref:`fr <usx-note_footnote_charstyle_fr>`
* :ref:`ft <usx-note_footnote_charstyle_ft>`
* :ref:`fk <usx-note_footnote_charstyle_fk>`
* :ref:`fq <usx-note_footnote_charstyle_fq>`
* :ref:`fqa <usx-note_footnote_charstyle_fqa>`
* :ref:`fl <usx-note_footnote_charstyle_fl>`
* :ref:`fp <usx-note_footnote_charstyle_fp>`
* :ref:`fv <usx-note_footnote_charstyle_fv>`
* :ref:`fdc <usx-note_footnote_charstyle_fdc>`
 
-----

.. _usx-note_footnote_charstyle_fr:

:@style: fr
:Use: Footnote "origin" reference. |br|
	This is the chapter and verse(s) that note refers to.
:Valid In: Any :ref:`usx-note_footnote_char`

.. code-block:: xml

	<note caller="+" style="f">
	  <char style="fr">1.1: </char>
	  <char style="ft">Some manuscripts do not have </char>
	  <char style="fq">the Son of God.</char>
	</note>

-----

.. _usx-note_footnote_charstyle_ft:

:@style: ft
:Use: Footnote text |br|
	The primary (explanatory) text of the footnote.
:Valid In: Any :ref:`usx-note_footnote_char`

-----

.. _usx-note_footnote_charstyle_fk:

:@style: fk
:Use: A specific keyword/term from the text for which the footnote is being provided.
:Valid In: Any :ref:`usx-note_footnote_char`

	.. image:: images/usx-notechar-style_fk.jpg
		:width: 450px

.. code-block:: xml

	<note caller="+" style="f">
	  <char style="fr">3.20: </char>
	  <char style="fk">Adam </char>
	  <char style="ft">This name in Hebrew means "all human beings."</char>
	</note>		

-----

.. _usx-note_footnote_charstyle_fq:

:@style: Footnote translation quotation.
:Use: A quotation from the current scripture text translation for which the note is being provided. |br|
	Longer quotations are sometimes shortened using an ellipsis (i.e. suspension dots "...").
:Valid In: Any :ref:`usx-note_footnote_char`

	.. image:: images/usx-notechar-style_fq.jpg
		:width: 450px

.. code-block:: xml

	<note caller="+" style="f">
	  <char style="fr">1.1: </char>
	  <char style="ft">Some manuscripts do not have </char>
	  <char style="fq">the Son of God.</char>
	</note>

-----

.. _usx-note_footnote_charstyle_fqa:

:@style: fqa
:Use: Footnote alternate translation. |br|
	Used to distinguish between a quotation of the current scripture text translation, and an alternate translation.
:Valid In: Any :ref:`usx-note_footnote_char`

	.. image:: images/usx-notechar-style_fqa.jpg
		:width: 450px

.. code-block:: xml

	<note caller="+" style="f">
	  <char style="fr">1.4: </char>
	  <char style="fq">John appeared in the desert, baptizing and preaching; </char>
	  <char style="ft">some manuscripts have </char>
	  <char style="fqa">John the Baptist appeared in the desert, preaching.</char>
	</note>

-----

.. _usx-note_footnote_charstyle_fl:

:@style: fl
:Use: Footnote "label" text. |br|
	Can be used for marking or "labeling" a word or words which are used consistently across certain types of translation notes (such as the words "Or" in an alternative translation style note, "Others", "Heb.", "LXX" etc.).
:Valid In: Any :ref:`usx-note_footnote_char`

-----

.. _usx-note_footnote_charstyle_fp:

:@style: fp
:Use: Footnote additional paragraph. |br|
	Use this marker to if you need to indicate the start of a new paragraph within a footnote (uncommon).
:Valid In: Any :ref:`usx-note_footnote_char`

-----

.. _usx-note_footnote_charstyle_fv:

:@style: fv
:Use: Footnote verse number. |br|
	A verse number in the the text quotation or alternative translation.
:Valid In: Any :ref:`usx-note_footnote_char`

	.. image:: images/usx-notechar-style_fv.jpg
		:width: 500px

.. code-block:: xml

	<note caller="+" style="f">
	  <char style="fr">7.38: </char>
	  <char style="ft">Jesus' words in verses 37-38 may be translated: </char>
	  <char style="fqa">“Whoever is thirsty should come to me and drink. </char>
	  <char style="fv">38</char> As the scripture says, ‘Streams of life-giving water  
	  will pour out from within anyone who believes in me.’”
	</note>

-----

.. _usx-note_footnote_charstyle_fdc:

:@style: fdc
:Use: Material to be included only in publications that contain the Deuterocanonical/Apocrypha books.
:Valid In: Any :ref:`usx-note_footnote_char`

-----

.. note::

	Other :ref:`usx-element_char` :doc:`@style types <charstyles>` may be nested within any of the standard footnote :ref:`usx-element_char` :ref:`@style types <usx-note_footnote_charstyles>` shown in the list above.

.. index:: usx <note> (cross reference)
.. index:: usx <note> (study cross reference)
.. _usx-note_crossReference:

<note> (CrossReference)
-----------------------
|ico_R| Schema pattern name: **CrossReference**

:Element: note |br|
	*empty* (all content is contained within the note's child char elements)
:Added: 1.0
:Use: Contains child :ref:`usx-element_char` elements to contain the content for a cross reference or study cross reference.
:@caller: Cross reference caller. |req| |br|
	``+`` | ``-`` | <user defined caller> |br|
	*A <user defined caller> may be any single character or sequence of characters preferred as the caller for a note.*
:@style: Content (cross reference) type. |req| |br|
	``x`` (cross reference) | ``ex`` (extended / study cross reference)
:Valid in: :ref:`usx-div_bookTitles`, :ref:`usx-div_bookIntroduction`, :ref:`usx-div_introductionEndTitles`, :ref:`usx-div_chapterText`
:Parents: :ref:`usx-element_para`, :ref:`usx-element_char`, :ref:`usx-element_cell`

Diagram
"""""""

.. image:: images/usx-pattern_CrossReference.png

.. index:: usx <char> (cross reference)
.. _usx-note_crossReference_char:

<char> (CrossReference)
^^^^^^^^^^^^^^^^^^^^^^^
|ico_R| Schema pattern name: **CrossReferenceChar**

:Element: char |br|
	xsd:string
:Added: 1.0
:Use: An element for marking various cross reference content types.
:@style: Cross reference content type. |req| |br|
	The :ref:`usx-element_char` (Cross Reference) @style types list (below) presents an itemization of @style values valid within :ref:`usx-element_char` elements which are children of :ref:`usx-element_note` @style="x".
:Valid in: :ref:`usx-note_crossReference`

Diagram
"""""""

.. image:: images/usx-pattern_CrossReferenceChar.png

.. _usx-note_crossReference_charstyles:

<char> (Cross Reference) @style Types
"""""""""""""""""""""""""""""""""""""

* :ref:`xo <usx-note_crossReference_charstyle_xo>`
* :ref:`xt <usx-note_crossReference_charstyle_xt>`
* :ref:`xk <usx-note_crossReference_charstyle_xk>`
* :ref:`xq <usx-note_crossReference_charstyle_xq>`
* :ref:`xot <usx-note_crossReference_charstyle_xot>`
* :ref:`xnt <usx-note_crossReference_charstyle_xnt>`
* :ref:`xdc <usx-note_crossReference_charstyle_xdc>`

-----

.. _usx-note_crossReference_charstyle_xo:

:@style: xo
:Use: Cross reference origin reference. |br|
	This is the chapter and verse(s) that target (@style="xt") reference(s) are being provided for.
:Valid In: Any :ref:`usx-note_crossReference_char`

	.. image:: images/usx-notechar-style_xo.jpg
		:width: 500px

.. code-block:: xml

	<note caller="-" style="x">
	  <char style="xo">2.23: </char>
	  <char style="xt">Mk 1.24; Lk 2.39; Jn 1.45.</char>
	</note>

-----

.. _usx-note_crossReference_charstyle_xt:

:@style: xt
:Use: Cross reference target reference(s). |br|
	The list of target scripture passages being suggested as references for comparison/review with respect to the text (or concept) of the origin reference. |br|
	A list of book name abbreviations and chapter + verse references, separated by semicolons or other book list separator character.
:Valid In: Any :ref:`usx-note_crossReference_char`

-----

.. _usx-note_crossReference_charstyle_xk:

:@style: xk
:Use: A keyword from the scripture translation text which the target reference(s) also refer to.
:Valid In: Any :ref:`usx-note_crossReference_char`

-----

.. _usx-note_crossReference_charstyle_xq:

:@style: xq
:Use: A quotation from the scripture text. |br|
	*Use of a quotation would be intended to help the reader to understand the portion of text (or concept) for which the target (xt) reference(s) are being supplied.*
:Valid In: Any :ref:`usx-note_crossReference_char`

-----

.. _usx-note_crossReference_charstyle_xot:

:@style: xot
:Use: References (or other text) which only to be included in publications that contain the Old Testament books.
:Valid In: Any :ref:`usx-note_crossReference_char`

-----

.. _usx-note_crossReference_charstyle_xnt:

:@style: xnt
:Use: References (or other text) which only to be included in publications that contain the New Testament books.
:Valid In: Any :ref:`usx-note_crossReference_char`

-----

.. _usx-note_crossReference_charstyle_xdc:

:@style: xdc
:Use: References (or other text) which only to be included in publications that contain the Deuterocanonical/Apocrypha books.
:Valid In: Any :ref:`usx-note_crossReference_char`

.. code-block:: xml

	<note caller="-" style="x">
	  <char style="xo">1.26: </char>
	  <char style="xdc">Ws 2.23; Si 17.3,4;</char>
	  <char style="xt">1 Co 11.7.</char>
	</note>
