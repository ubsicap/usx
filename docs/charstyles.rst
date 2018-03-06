.. include:: /_static/inc_styles.txt

.. index:: attribute; char@style
.. _usx-charstyles:

<char> @style Types
===================

.. note:: **@style types for** :ref:`usx-element_char` **elements occurring within** :ref:`usx-element_note`

	An additional list of :ref:`usx-element_char` @style types are defined for use in the context of footnotes and cross references. These are described in this document together with the definitions for the :ref:`usx-element_note` elements used for footnotes and cross references.

-----

.. index:: element; <char> (special text)
.. _usx-charstyles_specialText:

Special Text
------------

.. index:: char@style; add
.. _usx-charstyle_add:

add
^^^

:@style: add
:Use: Translator's addition. |br|
	Words added by the translator for clarity – text which is not literally a part of the original language, but which was supplied to make the meaning of the original clear.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Genesis 5.29 (Russian Synodal, Protestant Version)

.. image:: images/usx-char-style_add.jpg
	:width: 250px

-----

.. index:: char@style; bk
.. _usx-charstyle_bk:

bk
^^

:@style: bk
:Use: Quoted book title.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Introduction to Mark (GNT)

.. image:: images/usx-char-style_bk.jpg
	:width: 250px

-----

.. index:: char@style; dc
.. _usx-charstyle_dc:

dc
^^

:@style: dc
:Use: Deuterocanonical/LXX additions or insertions in the Protocanonical text. |br|
	General purpose use of <char> @style :ref:`dc <usx-charstyle_dc>` is encouraged wherever DC-only content is being marked. Use of context-specific DC-only markup (i.e. <char> @style :ref:`fdc <usx-note_footnote_charstyle_fdc>`, or :ref:`xdc <usx-note_crossReference_charstyle_xdc>`) is discouraged.
:Valid In: Any valid :ref:`usx-element_char`

**Text Samples** - Hebrews 1.3 (Spanish DHE - footnote)

.. code-block:: xml
	:name: usx-charstyle_dc_example
	:emphasize-lines: 6

	<verse number="3" style="v" />Él es el resplandor glorioso de Dios,
	<note caller="c" style="f">
		<char style="fr">1.3: </char>
		<char style="fk">Resplandor: </char>
		<char style="ft">Cf. Jn 1.4-9,14
		<char style="dc"> ; también Sab 7.25-26, donde algo parecido se dice de 
		la sabiduría</char></char>
	</note>

Psalm 115.3-4 (GNT - cross references)

.. code-block:: xml
	:name: usx-charstyle_dc_example2
	:emphasize-lines: 9

	<para style="q1">
		<verse number="3" style="v" />Our God is in heaven;
	<para style="q2">he does whatever he wishes.</para>
	<para style="q1">
		<verse number="4" style="v" />
		<note caller="-" style="x">
			<char style="xo">115.4-8: </char>
			<char style="xt">Ps 135.15-18; 
			<char style="dc"> Ltj Jr 4-73;</char> Rev 9.20.</char>
		</note>Their gods are made of silver and gold,</para>
	<para style="q2">formed by human hands.</para>

1 Corinthians 15.51-52 (GNT - cross reference)

.. code-block:: xml
	:name: usx-charstyle_dc_example3
	:emphasize-lines: 6

	<para style="p">
		<verse number="51-52" style="v" />
		<note caller="-" style="x">
			<char style="xo">15.51,52: </char>
			<char style="xt">
			<char style="dc">2Es 6.23; </char>
			1Th 4.15-17.
		</note>Listen to this secret truth: we shall not all die, but when the last trumpet sounds, 
	we shall all be changed in an instant, as quickly as the blinking of an eye. For when the trumpet 
	sounds, the dead will be raised, never to die again, and we shall all be changed.

-----

.. index:: char@style; ior, introductions; outline reference range
.. _usx-charstyle_ior:

ior
^^^

:@style: ior
:Use: Introduction outline reference range. |br|
	An :ref:`introduction outline entry <usx-parastyle_io>` typically ends with a range of references, sometimes within parentheses. This is an optional char style for marking these references separately.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Mark (CEV)

.. image:: images/usx-char-style_ior.jpg
	:width: 300px

-----

.. index:: char@style; iqt, introductions; quoted text
.. _usx-charstyle_iqt:

iqt
^^^

:@style: iqt
:Use: Introduction quoted text. |br|
	Scripture quotations, or other quoted text, appearing in the :ref:`usx-div_bookIntroduction`.
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. index:: char@style; k
.. _usx-charstyle_k:

k
^

:@style: k
:Use: Keyword / keyterm.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; litl
.. _usx-charstyle_litl:

litl
^^^^

|badge_3.0|

:@style: litl
:Added: 3.0
:Use: List entry total. |br|
	Use in “accounting” lists for denoting the total component of the text within a list item (<para> @style :ref:`li <usx-parastyle_li>`). An alternative to using :ref:`table <usx-element_table>` for the same content.
:Valid In: Any valid :ref:`usx-element_char` within <para> @style :ref:`li# <usx-parastyle_li>`

**Text and Formatting Sample** - Nehemiah 7.6-14 (GNT - *markup adapted*)

.. code-block:: xml
	:name: usx-char-style_litl_example
	:emphasize-lines: 10,12,14,16,18,20,22

	<para style="pm"><verse number="6" style="v" />These are the people of the province who came up 
		from the captivity of the exiles whom Nebuchadnezzar king of Babylon had taken captive (they 
		returned to Jerusalem and Judah, each to his own town, <verse number="7" style="v" />in 
		company with Zerubbabel, Jeshua, Nehemiah, Azariah, Raamiah, Nahamani, Mordecai, Bilshan, 
		Mispereth, Bigvai, Nehum and Baanah):</para>
	<para style="b" />
	<para style="pm">The list of the men of Israel:
	<para style="b" />
	<para style="lim1"><verse number="8" style="v" />the descendants of Parosh - 
		<char style="litl">2,172</char></para>
	<para style="lim1"><verse number="9" style="v" />of Shephatiah - 
		<char style="litl">372</char></para>
	<para style="lim1"><verse number="10" style="v" />of Arah - 
		<char style="litl">652</char></para>
	<para style="lim1"><verse number="11" style="v" />of Pahath-Moab (through the line of Jeshua 
		and Joab) - <char style="litl">2,818</char></para>
	<para style="lim1"><verse number="12" style="v" />of Elam - 
		<char style="litl">1,254</char></para>
	<para style="lim1"><verse number="13" style="v" />of Zattu - 
		<char style="litl">845</char></para>
	<para style="lim1"><verse number="14" style="v" />of Zaccai - 
		<char style="litl">760</char></para>
	...

.. image:: images/usx-char-style_litl.jpg
	:width: 250px

-----

.. index:: char@style; nd
.. _usx-charstyle_nd:

nd
^^

:@style: nd
:Use: Name of God (name of deity).
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Exodus 3.15 (GNT)

.. image:: images/usx-char-style_nd.jpg
	:width: 250px

-----

.. index:: char@style; ord
.. _usx-charstyle_ord:

ord
^^^

:@style: ord
:Use: Ordinal number ending (i.e. in 1st — ``1<char style="ord">st</char>``).
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; pn
.. _usx-charstyle_pn:

pn
^^

:@style: pn
:Use: Proper name.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; png
.. _usx-charstyle_png:

png
^^^

|badge_3.0|

:@style: png
:Added: 3.0
:Use: Geographic proper name. |br|
	Particularly in China, there are various groups which have the practice of distinguishing visually between proper names of people and proper names of geographic places in published texts. Published materials may use a single underline to present proper names of people, and double underline to present proper names of geographic places. Alternatively, dotted underlines have been used for geographic proper names. |br| |br|
	Special presentation for names can assist readers to know what the text means, especially readers who may struggle with reading skills and may be overloaded by the transliterated names.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; qac, poetry; acrostic letter
.. _usx-charstyle_qac:

qac
^^^

:@style: qac
:Use: Used to indicate the acrostic letter within a poetic line.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Lamentations 1.1,2 (Spanish TLA)

.. image:: images/usx-char-style_qac.jpg
	:width: 250px

-----

.. index:: char@style; qs, poetry; selah text
.. _usx-charstyle_qs:

qs
^^

:@style: qs
:Use: Used for the expression "Selah" commonly found in Psalms and Habakkuk. |br|
	This text is frequently right aligned, and rendered on the same line as the previous poetic text, if space allows.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Psalm 3.2 (NRSV)

.. image:: images/usx-char-style_qs.jpg
	:width: 250px

-----

.. index:: char@style; qt
.. _usx-charstyle_qt:

qt
^^

:@style: qt
:Use: Quoted text. |br|
	Old Testament quotations in the New Testament, or other quotations.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Mark 1.2-3 (GNT)

.. image:: images/usx-char-style_qt.jpg
	:width: 250px

-----

.. index:: char@style; rq
.. _usx-charstyle_rq:

rq
^^

:@style: rq
:Use: Inline quotation reference(s). |br|
	A reference indicating the source text for the preceding quotation (usually an Old Testament quote). |br|
	The reference(s) are intended to be formatted within the scripture body text column, and not extracted from the text as are regular :ref:`cross-references <usx-note_CrossReference>`. They are also typically separated from the main text of Scripture using a different type style and alignment.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Hebrews 1.5 (GNT)

.. image:: images/usx-char-style_rq.jpg
	:width: 250px

-----

.. index:: char@style; sig
.. _usx-charstyle_sig:

sig
^^^

:@style: sig
:Use: Signature of the author of an epistle.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Colossians 4.18 (GNT)

.. image:: images/usx-char-style_sig.jpg
	:width: 250px

-----

.. index:: char@style; sls
.. _usx-charstyle_sls:

sls
^^^

:@style: sls
:Use: Passage of text based on a secondary language or alternate text source. |br|
	For example: The Nouvelle Bible Segond 2002 (NBS02) has large sections of text in EZR and DAN in italics, to represent where the original text is in Aramaic, not Hebrew.
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Ezra 4.8—6.18 (NBS - French, Nouvelle Bible Segond)

.. image:: images/usx-char-style_sls.jpg
	:width: 250px

-----

.. index:: char@style; tl
.. _usx-charstyle_tl:

tl
^^

:@style: tl
:Use: Transliterated (or foreign) word(s).
:Valid In: Any valid :ref:`usx-element_char`

**Formatting Sample** - Matthew 27.46 (GNT)

.. image:: images/usx-char-style_tl.jpg
	:width: 250px

-----

.. index:: char@style; wj
.. _usx-charstyle_wj:

wj
^^

:@style: wj
:Use: Words of Jesus.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: element; <char> (character styles)
.. _usx-charstyles_characterStyles:

Character Styling
-----------------

.. index:: char@style; em
.. _usx-charstyle_em:

em
^^

:@style: em
:Use: Emphasis text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; bd
.. _usx-charstyle_bd:

bd
^^

:@style: bd
:Use: Bold text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; bdit
.. _usx-charstyle_bdit:

bdit
^^^^

:@style: bdit
:Use: Bold + Italic text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; it
.. _usx-charstyle_it:

it
^^

:@style: it
:Use: Italic text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; no
.. _usx-charstyle_no:

no
^^

:@style: no
:Use: Normal text. |br|
	May be used when a containing paragraph element may be set in an alternate font style (e.g. italic), and a selection of text should instead be displayed in normal style.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; sc
.. _usx-charstyle_sc:

sc
^^

:@style: sc
:Use: Small-cap text.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: element; <char> (spacing and breaks)
.. _usx-charstyles_spacingBreaks:

Spacing and Breaks
------------------

Discretionary (optional) line break location. See element :ref:`optbreak <usx-element_optbreak>`.

-----

.. index:: element; <char> (special features)
.. _usx-charstyles_specialFeatures:

Special Features
----------------

.. index:: char@style; rb, ruby glossing
.. _usx-charstyle_rb:

rb
^^

:@style: rb
:Use: Ruby glossing. |br|
	Used to mark the base text being annotated with ruby characters.
:Valid In: Any valid :ref:`usx-element_char`

.. note::

	**About Ruby**
	|ico_See| *See:* https://www.w3.org/TR/ruby/

	**Han characters:** Chinese, Japanese, and Korean texts have some characters that they share in common. In Japanese these are called Kanji (literally “Han characters”). There are several thousand of these characters to learn. For new readers or readers new to the Biblical texts it may be very difficult for them to recognize what Chinese or Japanese word corresponds to the Han character(s) they are seeing.

	**Ruby glosses:** In order to help these readers, some Bibles are printed with glosses using small phonetic characters (e.g. Japanese uses the hiragana alphabet) placed above the more symbolic Han characters to tell the reader how to pronounce the character. These phonetic characters are generically called "ruby glosses" or "rubies". In Japanese this technique is called Furigana.

.. _usx-charstyle_rb-attr:
.. index:: attribute; char@gloss (@style="rb"), ruby glossing; attributes

.. rubric:: Attributes |ico_Tag|

|badge_3.0|

*Additional* :doc:`attributes <attributes>` for :ref:`<char> <usx-element_char>` which can be used in this context.

:@gloss: Ruby glosses |br|
	Use a colon ``:`` to separate multiple elements for glossing each of the characters within a base text phrase.

For example: If the base text being glossed is a phrase of two Han characters (B), then the ruby gloss text (gg) may contain two elements, one for glossing each of the base text characters making up the phrase.

.. code-block:: xml

	<char style="rb" gloss="gg:gg">BB</char>

This syntax allows the decision to present glosses by phrase or by group to be made at the publication stage, rather than pre-determined during translation.

Parts of a phrase gloss may be left empty. In the example phrase below the second and fourth base characters are unglossed:

.. code-block:: xml

	<char style="rb" gloss="g1::g3:">BBBB</char>

**Text and Formatting Samples**

1. One Han character with a single ruby gloss.

.. code-block:: xml

	<char style="rb" gloss="あい">哀</char>

2. Two Han characters with a single ruby phrase gloss

.. code-block:: xml

	<char style="rb" gloss="はなはなし">話賄</char>

3. Phrase gloss broken down into individual pieces by adding colons between ruby characters

.. code-block:: xml

	<char style="rb" gloss="はな:はなし">話賄</char>

4. A character sequence which includes non-Han characters (hiragana), which are NOT glossed.

.. code-block:: xml

	<char style="rb" gloss="さだ:">定ま</char>

5. An un-glossed character occurring between glossed characters in the "phrase".

.. code-block:: xml

	<char style="rb" gloss="かみ::こ">神の子</char>

Genesis 1.1-2 (Japanes Living Bible - Biblica)

.. code-block:: xml
	:name: usx-char-style_rb_example

	<para style="p"><verse number="1" style="v" />まだ<char style="rb" gloss="なに">何</char>
		もなかった<char style="rb" gloss="とき">時</char>、<char style="rb" gloss="かみ">神</char>は
		<char style="rb" gloss="てん">天</char>と<char style="rb" gloss="ち">地</char>を
		<char style="rb" gloss="つく">造</char>りました。
		<verse number="2" style="v" /><char style="rb" gloss="ち">地</char>は
		<char style="rb" gloss="かたち">形</char>も<char style="rb" gloss="さだ">定</char>まらず、
		<char style="rb" gloss="やみ">闇</char>に<char style="rb" gloss="つつ">包</char>まれた
		<char style="rb" gloss="みず">水</char>の<char style="rb" gloss="うえ">上</char>を、さらに
		<char style="rb" gloss="かみ">神</char>の<char style="rb" gloss="れい">霊</char>が
		<char style="rb" gloss="おお">覆</char>っていました。</para>

.. image:: images/usx-char-style_rb.jpg
	:width: 300px

-----

.. index:: char@style; pro
.. _usx-charstyle_pro:

pro
^^^

:@style: pro
:Use: Pronunciation information |br|
	*Used for CJK texts.*
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; w
.. _usx-charstyle_w:

w
^

:@style: w
:Use: Wordlist/glossary/dictionary entry. |br|
	Surround word(s) with this char style to indicate that it appears (or should appear) in a published word list/glossary.
:Valid In: Any valid :ref:`usx-element_char`

.. _usx-charstyle_w-attr:
.. index:: attribute; char@lemma (@style="w"), wordlist entry; attributes

.. rubric:: Attributes |ico_Tag|

|badge_3.0|

*Additional* :doc:`attributes <attributes>` for :ref:`<char> <usx-element_char>` which can be used in this context.

:@lemma: Citation form for the term in the glossary

.. code-block:: xml

    <char style="w" lemma="grace">gracious</char>

.. index:: attribute; char@strong (@style="w")

:@strong: Strong’s ID in the form ``H#####`` (Hebrew) or ``G#####`` (Greek) |br| |br|
	A strong's ID **augmentation** identifier, if required, should be separated from the strong value by a colon ``:``

.. code-block:: xml

	<char style="w" lemma="grace" strong="G05485">gracious</char>
	<char style="w" strong="G05485">gracious</char>
	<char style="w" strong="H01234,G05485">gracious</char>
	
	<char style="w" strong="G05485:a">gracious</char>

.. index:: attribute; char@srcloc (@style="w")

:@srcloc: Location of the word in the source text; Example: GNT version 5 text, book 51, chapter 1, verse 2, word 1.

.. code-block:: xml

	<char style="w" lemma="grace" srcloc="gnt5:51.1.2.1">gracious</char>

-----

.. index:: char@style; wg
.. _usx-charstyle_wg:

wg
^^

:@style: wg
:Use: Greek word list entry.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; wh
.. _usx-charstyle_wh:

wh
^^

:@style: wh
:Use: Hebrew word list entry.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: char@style; wa
.. _usx-charstyle_wa:

wa
^^

|badge_3.0|

:@style: wa
:Added: 3.0
:Use: Aramaic word list entry.
:Valid In: Any valid :ref:`usx-element_char`

-----

.. index:: element; <char> (structured lists)
.. _usx-charstyles_structuredLists:

Structured List Entries
-----------------------

|badge_3.0|

Standard USX :ref:`table <usx-element_table>` structures can be challenging to display on small page sizes, or digital device displays. Scripture content is sometimes encoded within a USX table in order to suggest a meaningful presentation, but the encoded presentation may only be rendered accurately or legibly in a larger format. The following <char> @style types can be used to create structured list entries which identify a set of related content, but do not encode a specific presentation.

.. note::

	Structured lists are not strictly a replacement for table markup, but may prove to be a more flexible option for some types of tabular content.

<char> @style types :ref:`lik <usx-charstyle_lik>` and :ref:`liv# <usx-charstyle_liv>` mark the content of list entries (<para> @style :ref:`li# <usx-parastyle_li>`) which are essentially a key + value pair. A key may have multiple values.

-----

.. index:: char@style; lik
.. _usx-charstyle_lik:

lik
^^^

|badge_3.0|

:@style: lik
:Added: 3.0
:Use: List entry "key" content.
:Valid In: Any valid :ref:`usx-element_char` within <para> @style :ref:`li# <usx-parastyle_li>`

-----

.. index:: char@style; liv
.. _usx-charstyle_liv:

liv#
^^^^

|badge_3.0|

:@style: liv#
:Added: 3.0
:Use: List entry "value" content. |br|
	The variable # represents the sequence of the marked item in a list entry with multiple values. |br|
	**liv = liv1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: Any valid :ref:`usx-element_char` within <para> @style :ref:`li# <usx-parastyle_li>`

**Text and Formatting Sample** - 1 Chronicles 27:16-22 (GNT - *markup adapted*)

.. code-block:: xml
	:name: usx-char-style_lik_liv_example
	:emphasize-lines: 5,7,9,11,13,16,18,20,22,24,26,28,30

	<para style="s1">Administration of the Tribes of Israel</para>
	<para style="lh"><verse number="16-22" style="v" />This is the list of the administrators 
		of the tribes of Israel:</para>
	<para style="li1">
		<char style="lik">Reuben</char> <char style="liv1">Eliezer son of Zichri</char></para>
	<para style="li1">
		<char style="lik">Simeon</char> <char style="liv1">Shephatiah son of Maacah</char></para>
	<para style="li1">
		<char style="lik">Levi</char> <char style="liv1">Hashabiah son of Kemuel</char></para>
	<para style="li1">
		<char style="lik">Aaron</char> <char style="liv1">Zadok</char></para>
	<para style="li1">
		<char style="lik">Judah</char> <char style="liv1">Elihu, one of King David's brothers</char>
		</para>
	<para style="li1">
		<char style="lik">Issachar</char> <char style="liv1">Omri son of Michael</char></para>
	<para style="li1">
		<char style="lik">Zebulun</char> <char style="liv1">Ishmaiah son of Obadiah</char></para>
	<para style="li1">
		<char style="lik">Naphtali</char> <char style="liv1">Jeremoth son of Azriel</char></para>
	<para style="li1">
		<char style="lik">Ephraim</char> <char style="liv1">Hoshea son of Azaziah</char></para>
	<para style="li1">
		<char style="lik">West Manasseh</char> <char style="liv1">Joel son of Pedaiah</char></para>
	<para style="li1">
		<char style="lik">East Manasseh</char> <char style="liv1">Iddo son of Zechariah</char></para>
	<para style="li1">
		<char style="lik">Benjamin</char> <char style="liv1">Jaasiel son of Abner</char></para>
	<para style="li1">
		<char style="lik">Dan</char> <char style="liv1">Azarel son of Jeroham</char></para>
	<para style="lf">This was the list of the administrators of the tribes of Israel.</para>

.. image:: images/usx-char-style_lik_liv.jpg
	:width: 250px

-----

.. index:: element; <char> (linking)
.. _usx-charstyles_linking:

Linking
-------

.. index:: char@style; jmp
.. _usx-charstyle_jmp:

jmp
^^^

|badge_3.0|

:@style: jmp
:Added: 3.0
:Use: Available for associating :doc:`linking attributes <linking>` to a span of text when no other :ref:`<char> <usx-element_char>` element is already applied to the text at this location.
:Valid In: Any valid :ref:`usx-element_char`

|ico_See| See: :doc:`Linking Attributes <linking>`.