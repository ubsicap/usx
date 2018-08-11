.. include:: /_static/inc_styles.txt

.. index:: char @style
.. _usx-charstyles:

<char> @style Types
===================

.. contents::

-----

.. note:: **@style types for** :ref:`usx-element_char` **elements occurring within** :ref:`usx-element_note`

	An additional list of :ref:`usx-element_char` @style types are defined for use in the context of footnotes and cross references. These are described in this document together with the definitions for the :ref:`usx-element_note` elements used for footnotes and cross references.

.. index:: usx <char> (special text)
.. _usx-charstyles_specialText:

Special Text
------------
* :ref:`ior <usx-charstyle_ior>`
* :ref:`iqt <usx-charstyle_iqt>`
* :ref:`add <usx-charstyle_add>`
* :ref:`bk <usx-charstyle_bk>`
* :ref:`dc <usx-charstyle_dc>`
* :ref:`k <usx-charstyle_k>`
* :ref:`nd <usx-charstyle_nd>`
* :ref:`ord <usx-charstyle_ord>`
* :ref:`pn <usx-charstyle_pn>`
* :ref:`qac <usx-charstyle_qac>`
* :ref:`qs <usx-charstyle_qs>`
* :ref:`qt <usx-charstyle_qt>`
* :ref:`rq <usx-charstyle_rq>`
* :ref:`sig <usx-charstyle_sig>`
* :ref:`sls <usx-charstyle_sls>`
* :ref:`tl <usx-charstyle_tl>`
* :ref:`wj <usx-charstyle_wj>`

-----

.. _usx-charstyle_ior:
.. index:: char @style (ior)

:@style: ior
:Use: Introduction outline reference range. |br|
	An :ref:`introduction outline entry <usx-parastyle_io>` typically ends with a range of references, sometimes within parentheses. This is an optional char style for marking these references separately.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-char-style_ior.jpg
		:width: 300px

-----

.. _usx-charstyle_iqt:
.. index:: char @style (iqt)

:@style: iqt
:Use: Introduction quoted text. |br|
	Scripture quotations, or other quoted text, appearing in the :ref:`usx-div_bookIntroduction`.
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-charstyle_add:
.. index:: char @style (add)

:@style: add
:Use: Translator's addition. |br|
	Words added by the translator for clarity – text which is not literally a part of the original language, but which was supplied to make the meaning of the original clear.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_add.jpg
		:width: 250px

-----

.. _usx-charstyle_bk:
.. index:: char @style (bk)

:@style: bk
:Use: Quoted book title.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_bk.jpg
		:width: 250px

-----

.. _usx-charstyle_dc:
.. index:: char @style (dc)

:@style: dc
:Use: Deuterocanonical/LXX additions or insertions in the Protocanonical text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_k:
.. index:: char @style (k)

:@style: k
:Use: Keyword / keyterm.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_nd:
.. index:: char @style (nd)

:@style: nd
:Use: Name of God (name of deity).
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_nd.jpg
		:width: 250px

-----

.. _usx-charstyle_ord:
.. index:: char @style (ord)

:@style: ord
:Use: Ordinal number ending (i.e. in 1st — ``1<char style="ord">st</char>``).
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_pn:
.. index:: char @style (pn)

:@style: pn
:Use: Proper name.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_qac:
.. index:: char @style (qac)

:@style: qac
:Use: Used to indicate the acrostic letter within a poetic line.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_qac.jpg
		:width: 250px

-----

.. _usx-charstyle_qs:
.. index:: char @style (qs)

:@style: qs
:Use: Used for the expression "Selah" commonly found in Psalms and Habakkuk. |br|
	This text is frequently right aligned, and rendered on the same line as the previous poetic text, if space allows.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_qs.jpg
		:width: 250px

-----

.. _usx-charstyle_qt:
.. index:: char @style (qt)

:@style: qt
:Use: Quoted text. |br|
	Old Testament quotations in the New Testament, or other quotations.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_qt.jpg
		:width: 250px

-----

.. _usx-charstyle_rq:
.. index:: char @style (rq)

:@style: rq
:Use: Inline quotation reference(s). |br|
	A reference indicating the source text for the preceding quotation (usually an Old Testament quote). |br|
	The reference(s) are intended to be formatted within the scripture body text column, and not extracted from the text as are regular :ref:`cross-references <usx-note_CrossReference>`. They are also typically separated from the main text of Scripture using a different type style and alignment.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_rq.jpg
		:width: 250px

-----

.. _usx-charstyle_sig:
.. index:: char @style (sig)

:@style: sig
:Use: Signature of the author of an epistle.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_sig.jpg
		:width: 250px

-----

.. _usx-charstyle_sls:
.. index:: char @style (sls)

:@style: sls
:Use: Passage of text based on a secondary language or alternate text source. |br|
	For example: The Nouvelle Bible Segond 2002 (NBS02) has large sections of text in EZR and DAN in italics, to represent where the original text is in Aramaic, not Hebrew.
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_sls.jpg
		:width: 250px

-----

.. _usx-charstyle_tl:
.. index:: char @style (tl)

:@style: tl
:Use: Transliterated (or foreign) word(s).
:Valid In: Any valid :ref:`usx-element_char`

	.. image:: images/usx-char-style_tl.jpg
		:width: 250px

-----

.. _usx-charstyle_wj:
.. index:: char @style (wj)

:@style: wj
:Use: Words of Jesus.
:Valid In: Any valid :ref:`usx-element_char`

.. index:: usx <char> (character styles)
.. _usx-charstyles_characterStyles:

Character Styling
-----------------
* :ref:`bd <usx-charstyle_bd>`
* :ref:`bdit <usx-charstyle_bdit>`
* :ref:`em <usx-charstyle_em>`
* :ref:`it <usx-charstyle_it>`
* :ref:`no <usx-charstyle_no>`
* :ref:`sc <usx-charstyle_sc>`

-----

.. _usx-charstyle_bd:
.. index:: char @style (bd)

:@style: bd
:Use: Bold text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_bdit:
.. index:: char @style (bdit)

:@style: bdit
:Use: Bold + Italic text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_em:
.. index:: char @style (em)

:@style: em
:Use: Emphasis text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_it:
.. index:: char @style (it)

:@style: it
:Use: Italic text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_no:
.. index:: char @style (no)

:@style: no
:Use: Normal text. |br|
	May be used when a containing paragraph element may be set in an alternate font style (e.g. italic), and a selection of text should instead be displayed in normal style.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_sc:
.. index:: char @style (sc)

:@style: sc
:Use: Small-cap text.
:Valid In: Any valid :ref:`usx-element_char`

.. index:: usx <char> (special features)
.. _usx-charstyles_specialFeatures:

Special Features
----------------
* pro
* w
* wg
* wh

-----

.. _usx-charstyle_pro:
.. index:: char @style (pro)

:@style: pro
:Use: Pronunciation information |br|
	*Used for CJK texts.*
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_w:
.. index:: char @style (w)

:@style: w
:Use: Wordlist/glossary/dictionary entry. |br|
	Surround word(s) with this char style to indicate that it appears (or should appear) in a published word list/glossary.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_wg:
.. index:: char @style (wg)

:@style: wg
:Use: Greek word list entry.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. _usx-charstyle_wh:
.. index:: char @style (wh)

:@style: wh
:Use: Hebrew word list entry.
:Valid In: Any valid :ref:`usx-element_char`
