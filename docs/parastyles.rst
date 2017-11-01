.. include:: /_static/inc_styles.txt

.. index:: para @style
.. _usx-parastyles:

<para> @style Types
===================

.. contents::
	:depth: 2

-----

.. _usx-notes_numberedStyles:

.. note:: **Numbered <para> @style Attributes**

	Some @style attributes include an optional numeric variable, which is represented in this documentation by a hash character (#). In USX the attribute number indicates:

	* A portion of a complete element, or relative weighting of the "pieces" of the elements, such as \mt1, \mt2, \mt3 which are all parts of a major title.
	* The level of division (hierarchy).
	* The level of indentation relative to other like elements, as in poetry (q#) or lists (li#) or outlines (io#).
	
	**style = style1** — The unnumbered version of a style attribute may be used when only one level of this paragraph style exists within the project text. Numbers should always be included when more than one level of the paragraph style exists within the project text.

-----

.. index:: usx <para> (identification)
.. _usx-parastyles_identification:

Identification
--------------

.. _usx-parastyle_h:
.. index:: para @style (h)

h
^

:@style: h
:Use: Running header text.
:Valid In: :ref:`usx-div_bookHeaders`

**Formatting Sample** - Matthew

.. image:: images/usx-para-style_h.jpg
	:width: 300px

-----

.. _usx-parastyle_toc1:
.. index:: para @style (toc1)

toc1
^^^^

:@style: toc1
:Use: Long table of contents text.
:Valid In: :ref:`usx-div_bookHeaders`

-----

.. _usx-parastyle_toc2:
.. index:: para @style (toc2)

toc2
^^^^

:@style: toc2
:Use: Short table of contents text.
:Valid In: :ref:`usx-div_bookHeaders`

-----

.. _usx-parastyle_toc3:
.. index:: para @style (toc3)

toc3
^^^^

:@style: toc3
:Use: Book abbreviation.
:Valid In: :ref:`usx-div_bookHeaders`

-----

.. note:: **About toc1, toc2, toc3**

	The `metadata.xml <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/metadata.html>`_ file within a DBL `text release bundle <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/index.html>`_ contains a `bookNames <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/metadata.html#booknames>`_ element in which each scripture book is itemized together with child elements for its long, short and abbreviated forms. The `bookNames <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/metadata.html#booknames>`_ element is the key location where this book naming metadata is contained within the bundle. USX para elements with attributes toc1, toc2, or toc3 are strictly optional data. Their presence in a USX file is valid, but reflects a legacy form of USFM markup in which the USFM files for each book were the key location for this book naming metadata.

.. index:: usx <para> (introductions)
.. _usx-parastyles_introductions:

-----

Introductions
-------------

.. _usx-parastyle_imt:
.. index:: para @style (imt)

imt#
^^^^

:@style: imt#
:Use: Introduction major title. |br|
	# denotes the title level or relative weighting. |br|
	**imt = imt1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Mark (RVE)

.. image:: images/usx-para-style_imt.jpg
	:width: 250px

-----

.. _usx-parastyle_is:
.. index:: para @style (is)

is#
^^^

:@style: is#
:Use: Introduction section heading. |br|
	# denotes the title level or relative weighting. |br|
	**is = is1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Mark (RVE)

.. image:: images/usx-para-style_is.jpg
	:width: 250px

-----

.. _usx-parastyle_ip:
.. index:: para @style (ip)

ip
^^

:@style: ip
:Use: Introduction paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** -  Introduction to Matthew (GNT)

.. image:: images/usx-para-style_ip.jpg
	:width: 250px

-----

.. _usx-parastyle_ipi:
.. index:: para @style (ipi)

ipi
^^^

:@style: ipi
:Use: Indented introduction paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to the Deuterocanonicals/Apocrypha (GCEV)

.. image:: images/usx-para-style_ipi.jpg
	:width: 250px

-----

.. _usx-parastyle_im:
.. index:: para @style (im)

im
^^^

:@style: im
:Use: Introduction flush left (margin) paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to the GCEV

.. image:: images/usx-para-style_im.jpg
	:width: 250px

-----

.. _usx-parastyle_imi:
.. index:: para @style (imi)

imi
^^^

:@style: imi
:Use: Indented introduction flush left (margin) paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to the GCEV

.. image:: images/usx-para-style_imi.jpg
	:width: 250px

-----

.. _usx-parastyle_ipq:
.. index:: para @style (ipq)

ipq
^^^

:@style: ipq
:Use: Introduction quote from scripture text paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Genesis (CEV)

.. image:: images/usx-para-style_ipq.jpg
	:width: 300px

-----

.. _usx-parastyle_imq:
.. index:: para @style (imq)

imq
^^^

:@style: imq
:Use: Introduction flush left (margin) quote from scripture text paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Genesis (CEV)

.. image:: images/usx-para-style_imq.jpg
	:width: 300px

-----

.. _usx-parastyle_ipr:
.. index:: para @style (ipr)

ipr
^^^

:@style: ipr
:Use: Introduction right-aligned paragraph. |br|
	Typically used for the reference for a quote from the scripture text (:ref:`imq <usx-parastyle_imq>`, :ref:`ipq <usx-parastyle_ipq>`)
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Genesis (CEV)

.. image:: images/usx-para-style_ipr.jpg
	:width: 250px

-----

.. _usx-parastyle_iq:
.. index:: para @style (iq)

iq#
^^^

:@style: iq#
:Use: Introduction poetic line. |br|
	# represents the level of indent (i.e. \iq1, \iq2, \iq3 etc.) |br|
	**iq = iq1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Titus (CEV)

.. image:: images/usx-para-style_iq.jpg
	:width: 250px

-----

.. _usx-parastyle_ib:
.. index:: para @style (ib)

ib
^^

:@style: ib
:Use: Introduction blank line. |br|
	May be used to explicitly indicate additional white space between paragraphs.
:Valid In: :ref:`usx-div_bookIntroduction`

|ico_See| *See also* :ref:`ipq <usx-parastyle_ipq>`, :ref:`imq <usx-parastyle_imq>` examples (above).

-----

.. _usx-parastyle_ili:
.. index:: para @style (ili)

ili#
^^^^

:@style: ili#
:Use: Introduction list item. |br|
	# represents the level of indent |br|
	**ili = ili1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Mark (Good News Study Bible)

.. image:: images/usx-para-style_ili.jpg
	:width: 250px

-----

.. _usx-parastyle_iot:
.. index:: para @style (iot)

iot
^^^

:@style: iot
:Use: Introduction outline title. (see :ref:`io# <usx-parastyle_io>` below)
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_io:
.. index:: para @style (io)

io#
^^^

:@style: io#
:Use: Introduction outline entry. |br|
	The outline entry typically ends with a range of references in parentheses. |br|
	References may be marked with char @style :ref:`ior <usx-charstyle_ior>`. |br|
	# represents the outline (indent) level.
	**io = io1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

**Formatting Sample** - Introduction to Mark (CEV)

.. image:: images/usx-para-style_io.jpg
	:width: 300px

-----

.. _usx-parastyle_iex:
.. index:: para @style (iex)

iex
^^^

:@style: iex
:Use: Introduction explanatory or bridge text (e.g. explanation of missing book in a short Old Testament). |br|
	*This para @style is used within Chapter Text.*
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_imte:
.. index:: para @style (imte)

imte
^^^^

:@style: imt#
:Use: Introduction major title ending. |br|
	Used to mark a major title indicating the end of the introduction. |br|
	# represents a portion of the title, with the lesser emphasis (relative weighting) being on the higher numbers. |br|
	**imte = imte1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_ie:
.. index:: para @style (ie)

ie
^^

:@style: ie
:Use: Introduction end. |br|
	Optionally included to explicitly indicate the end of the introduction material.
:Valid In: :ref:`usx-div_bookIntroduction`

.. index:: usx <para> (titles & headings)
.. _usx-parastyles_titles_headings:

-----

Titles and Headings
-------------------

.. _usx-parastyle_mt:
.. index:: para @style (mt)

mt#
^^^

:@style: mt#
:Use: Main title. |br|
	Key components in the title of a biblical book. |br|
	# represents a portion of the title, with the lesser emphasis (relative weighting) being on the higher numbers. |br|
	**mt = mt1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookTitles`

**Formatting Sample** - Introduction to Acts (GNT)

.. image:: images/usx-para-style_mt.jpg
	:width: 250px

Introduction to John (GNT)

.. image:: images/usx-para-style_mtAlt.jpg
	:width: 250px

-----

.. _usx-parastyle_mte:
.. index:: para @style (mte)

mte
^^^

:@style: mte#
:Use: Main title at introduction ending. |br|
	May be used in texts which repeat the main title at the end of the introduction.
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_cl:
.. index:: para @style (cl)

cl
^^

:@style: cl
:Use: The chapter "label" to be used when the chosen publishing presentation will render chapter divisions as headings (not drop cap numerals).
:Valid In: :ref:`usx-div_bookChapterLabel`, :ref:`usx-div_chapter`

.. note::

	**Usage note:** If <para @style="cl">Chapter Text</para> is added to the text once before chapter 1 it represents the vernacular text for the term "chapter" to be used throughout the current book. If <para @style="cl"> is added to the text after each individual <chapter> element, it represents the particular text to be used for the display of the current chapter heading (usually done if numbers are being presented as words, not numerals).

**Text and Formatting Samples** - Psalm 1 (GNT - *markup adapted* - general chapter label)

.. code-block:: xml
	:name: usx-para-style_cl_example
	:emphasize-lines: 1

	<para style="cl">Psalm</para>
	<chapter number="1" style="c" />
	<para style="s">True Happiness</para>
	<para style="q1">
	  <verse number="1" style="v" />Happy are those</para>
	<para style="q2">who reject the advice of evil people,</para>

.. image:: images/usx-para-style_cl.jpg
	:width: 250px

Psalm 1 (GNT - *markup adapted* - specific chapter label)

.. code-block:: xml
	:name: usx-para-style_cl_example-alt
	:emphasize-lines: 2

	<chapter number="1" style="c" />
	<para style="cl">Psalm One</para>
	<para style="s">True Happiness</para>
	<para style="q1">
	  <verse number="1" style="v" />Happy are those</para>
	<para style="q2">who reject the advice of evil people,</para>

.. image:: images/usx-para-style_cl-alt.jpg
	:width: 250px

-----

.. _usx-parastyle_cd:
.. index:: para @style (cd)

cd
^^

:@style: cd
:Use: Chapter description. |br|
	A brief description of chapter content (similar to :ref:`d <usx-parastyle_d>` - descriptive heading, or :ref:`iex <usx-parastyle_iex>` - introduction explanatory or bridge text).
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Genesis 1 (Russian Synodal, Protestant Version)

.. image:: images/usx-para-style_cd.jpg
	:width: 250px

-----

.. _usx-parastyle_ms:
.. index:: para @style (ms)

ms#
^^^

:@style: ms#
:Use: Major section heading.
	A heading added before a broader text division than what is typically considered a "section" division (see :ref:`s# <usx-parastyle_s>`). |br|
	# represents the level of division. |br|
	**ms = ms1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 1 (Book 1 division) (GNT)

.. image:: images/usx-para-style_ms.jpg
	:width: 250px

Daniel 1.1 (GNT)

.. image:: images/usx-para-style_msAlt.jpg
	:width: 250px

-----

.. _usx-parastyle_mr:
.. index:: para @style (mr)

mr
^^

:@style: mr
:Use: Major section reference range. |br|
	The text reference range listed under a major section heading.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 1 (Book 1 division) (GNT)

.. image:: images/usx-para-style_mr.jpg
	:width: 250px

-----

.. _usx-parastyle_s:
.. index:: para @style (s)

s#
^^

:@style: s#
:Use: Section heading. |br|
	The typical (common) section division heading. |br|
	# represents the level of division. |br|
	**s = s1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Proverbs 22.17 (GNT)

	*s1 example*

.. image:: images/usx-para-style_s1.jpg
	:width: 250px

Proverbs 22.22,24 (GNT) |br|
*s2 example*

.. image:: images/usx-para-style_s2.jpg
	:width: 250px

-----

.. _usx-parastyle_sr:
.. index:: para @style (sr)

sr
^^

:@style: sr
:Use: Section reference range. |br|
	The text reference range listed under a section heading. |br|
	sr is not equivalent to r which is used for marking parallel references. |br|
:See also: :ref:`mr <usx-parastyle_mr>`
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Proverbs 22.17 (GNT - *markup adapted*)

.. image:: images/usx-para-style_sr.jpg
	:width: 250px

-----

.. _usx-parastyle_r:
.. index:: para @style (r)

r
^

:@style: r
:Use: Parallel passage reference(s). |br|
	A reference to a parallel passage usually located under a section heading :ref:`s# <usx-parastyle_s>`. |br|
:See also: :doc:`char <charstyles>` @style :ref:`rq <usx-charstyle_rq>`.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Matthew 3.1 (GNT)

.. image:: images/usx-para-style_r.jpg
	:width: 250px

-----

.. _usx-parastyle_d:
.. index:: para @style (d)

d
^

:@style: d
:Use: Descriptive title (or "Hebrew subtitle"). |br|
	Sometimes used in Psalms under the section title (e.g. "For the director of Music").
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 3.1 (NRSV)

.. image:: images/usx-para-style_d.jpg
	:width: 250px

-----

.. _usx-parastyle_sp:
.. index:: para @style (sp)

sp
^^

:@style: sp
:Use: Speaker identification (e.g. Job and Song of Songs).
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Job 3.1 (GNT)

.. image:: images/usx-para-style_sp.jpg
	:width: 250px

.. index:: usx <para> (paragraphs)
.. _usx-parastyles_paragraphs:

-----

Paragraphs
----------

.. _usx-parastyle_p:
.. index:: para @style (p)

p
^

:@style: p
:Use: Normal paragraph.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Mark 1.1-4 (GNT)

.. image:: images/usx-para-style_p.jpg
	:width: 250px

-----

.. _usx-parastyle_m:
.. index:: para @style (m)

m
^

:@style: m
:Use: Margin paragraph. |br|
	Typically used to resume prose at the margin (without indent) after poetry or OT quotation (i.e. a continuation of the previous paragraph).
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Mark 12.37 (GNT)

.. image:: images/usx-para-style_m.jpg
	:width: 250px

-----

.. _usx-parastyle_po:
.. index:: para @style (po)

po
^^

|badge_3.0|

:@style: po
:Added: 3.0
:Use: Opening of an epistle / letter.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Romans 1.1,7 (GNT)

.. image:: images/usx-para-style_po.jpg
	:width: 450px

-----

.. _usx-parastyle_cls:
.. index:: para @style (cls)

cls
^^^

:@style: cls
:Use: Closure of an epistle / letter
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Colossians 4.18 (GNT - *markup adapated*)

.. image:: images/usx-para-style_cls.jpg
	:width: 250px

-----

.. _usx-parastyle_pmo:
.. index:: para @style (pmo)

pmo
^^^

:@style: pmo
:Use: Embedded text opening.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Acts 15.24 (CEV)

.. image:: images/usx-para-style_pmo.jpg
	:width: 250px

-----

.. _usx-parastyle_pm:
.. index:: para @style (pm)

pm
^^

:@style: pm
:Use: Embedded text paragraph.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Acts 15.24-27,28-29 (CEV)

.. image:: images/usx-para-style_pm.jpg
	:width: 250px

-----

.. _usx-parastyle_pmc:
.. index:: para @style (pmc)

pmc
^^^

:@style: pmc
:Use: Embedded text closing.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Acts 15.28-29 (CEV)

.. image:: images/usx-para-style_pmc.jpg
	:width: 250px

-----

.. _usx-parastyle_pmr:
.. index:: para @style (pmr)

pmr
^^^

:@style: pmr
:Use: Embedded text refrain.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Deuteronomy 27.15,16,17 (GNT - *markup adapted*)

.. image:: images/usx-para-style_pmr.jpg
	:width: 250px

-----

.. _usx-parastyle_pi:
.. index:: para @style (pi)

pi
^^

:@style: pi#
:Use: Indented paragraph. |br|
	Used in some texts for discourse sections. |br|
	# represents the level of indent. |br|
	**pi = pi1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:See also: :ref:`pm <usx-parastyle_pm>`
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Matthew 13.37-39 (CEV)

.. image:: images/usx-para-style_pi.jpg
	:width: 250px

-----

.. _usx-parastyle_mi:
.. index:: para @style (mi)

mi
^^

:@style: mi
:Use: Indented flush left paragraph
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Matthew 11.18-19 (CEV)

.. image:: images/usx-para-style_mi.jpg
	:width: 250px

-----

.. _usx-parastyle_pc:
.. index:: para @style (pc)

pc
^^

:@style: pc
:Use: Centered paragraph |br| |br|
	|ico_Cg| Recommended use: *Inscriptions* |br|
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Revelation 17.5 (CEV)

.. image:: images/usx-para-style_pc.jpg
	:width: 250px

-----

.. _usx-parastyle_pr:
.. index:: para @style (pr)

pr
^^

:@style: pr
:Use: Right-aligned paragraph |br| |br|
	|ico_W| Use is strongly discouraged. |br|
	|ico_Cg| Recommended alternate is :ref:`pmr <usx-parastyle_pmr>` |br|
:Valid In: :ref:`usx-div_chapter`

-----

.. _usx-parastyle_ph:
.. index:: para @style (ph)

ph#
^^^

:@style: ph#
:Use: Indented paragraph with hanging indent. |br|
	# represents the level of indent |br|
	**ph = ph1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes) |br| |br|
	|ico_W| Use is strongly discouraged. |br|
	|ico_Cg| Recommended alternate is :ref:`li# <usx-parastyle_li>` |br|
:Valid In: :ref:`usx-div_chapter`

-----

.. _usx-parastyle_lit:
.. index:: para @style (lit)

:@style: lit
:Use: Liturgical note/comment. (e.g. a guide which tells the reader/worshiper that he/she should recite a prayer or recitation etc.) |br|
	*In the formatting example image (below) the word Слава = "Glory"*
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 3 (Russian Synodal, Orthodox Version)

.. image:: images/usx-para-style_lit.jpg
	:width: 250px

.. index:: usx <para> (poetry)
.. _usx-parastyles_poetry:

-----

Poetry
------

.. _usx-parastyle_q:
.. index:: para @style (q)

q#
^^

:@style: q#
:Use: Poetic line. |br|
	# represents the level of indent (i.e. \q1, \q2, \q3 etc.).
	**q = q1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Habakkuk 3.1-2 (GNT)

.. image:: images/usx-para-style_q1.jpg
	:width: 250px

|br|

.. image:: images/usx-para-style_q2.jpg
	:width: 250px

-----

.. _usx-parastyle_qr:
.. index:: para @style (qr)

qr
^^

:@style: qr
:Use: Right-aligned poetic line. |br|
	|ico_Cg| Common use: Poetic refrain
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 136.1-3 (CEV - *markup adapated*)

.. image:: images/usx-para-style_qr.jpg
	:width: 250px

-----

.. _usx-parastyle_qc:
.. index:: para @style (qc)

qc
^^

:@style: qc
:Use: Centered poetic line.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 72.19 (GNT)

.. image:: images/usx-para-style_qc.jpg
	:width: 250px

-----

:@style: :ref:`qs <usx-charstyle_qs>`
:See: :doc:`char <charstyles>` @style :ref:`qs <usx-charstyle_qs>`

-----

.. _usx-parastyle_qa:
.. index:: para @style (qa)

qa
^^

:@style: qa
:Use: Acrostic heading.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 119 (NIV)

.. image:: images/usx-para-style_qa.jpg
	:width: 250px

-----

:@style: :ref:`qac <usx-charstyle_qac>`
:See: :doc:`char <charstyles>` @style :ref:`qac <usx-charstyle_qac>`

-----

.. _usx-parastyle_qm:
.. index:: para @style (qm)

qm#
^^^

:@style: qm#
:Use: Embedded text poetic line. |br|
	# represents the level of indent (i.e. \qm1, \qm2, etc.). |br|
	**qm = qm1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - 1 Chronicles 12.18 (GNT - *markup adapted*)

.. image:: images/usx-para-style_qm.jpg
	:width: 250px

-----

.. _usx-parastyle_b:
.. index:: para @style (b)

b
^

:@style: b
:Use: Blank line. |br|
	May be used to explicitly indicate additional white space between paragraphs. |br| |br|
	|ico_W| A para element with **b** style type should always be *empty*. |br|
	**b** should not be used before or after titles to indicate white-space.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Psalm 3 (GNT)

.. image:: images/usx-para-style_b.jpg
	:width: 250px

Habakkuk 3.1 (GNT)

.. image:: images/usx-para-style_bAlt.jpg
	:width: 250px

.. _usx-parastyle_lh:
.. index:: para @style (lh)

-----

Lists
-----

lh
^^

|badge_3.0|

:@style: lh
:Use: List header. |br|
	Some lists include an introductory and concluding remark (:ref:`lf <usx-parastyle_lf>`). They are an integral part of the list content, but are not list items. A list does not require either or both of these elements.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - 1 Chronicles 27:16-22 (GNT)

.. image:: images/usx-para-style_lh.jpg
	:width: 250px

.. _usx-parastyle_li:
.. index:: para @style (li)

-----

li#
^^^

:@style: li#
:Use: List entry. |br|
	An out-dented paragraph meant to highlight the items of a list. |br|
	# represents the level of indent |br|
	**li = li1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Numbers 7.84-88 (GNT)

.. image:: images/usx-para-style_li.jpg
	:width: 250px

.. _usx-parastyle_lf:
.. index:: para @style (lf)

-----

lf
^^

|badge_3.0|

:@style: lf
:Use: List footer. |br|
	Some lists include an introductory (:ref:`lh <usx-parastyle_lh>`) and concluding remark. They are an integral part of the list content, but are not list items. A list does not require either or both of these elements.
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - 1 Chronicles 27:16-22 (GNT)

.. image:: images/usx-para-style_lf.jpg
	:width: 250px

.. _usx-parastyle_lim:
.. index:: para @style (lim#)

-----

lim#
^^^^

|badge_3.0|

:@style: lim#
:Use: Embedded list entry. |br|
	An out-dented paragraph meant to highlight the items of an embedded list. |br|
	# represents the level of indent |br|
	**lim = lim1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes) |br|
	|ico_See| *See also* :ref:`li <usx-parastyle_li>`
:Valid In: :ref:`usx-div_chapter`

**Formatting Sample** - Nehemiah 7.4-25 (NIV)

.. image:: images/usx-para-style_lim.jpg
	:width: 250px