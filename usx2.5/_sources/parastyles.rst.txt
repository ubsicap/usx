.. include:: /_static/inc_styles.txt

.. index:: para @style
.. _usx-parastyles:

<para> @style Types
===================

.. contents::

-----

.. _usx-notes_numberedStyles:

.. note:: **Numbered <para> @style Attributes**

	Some @style attributes include an optional numeric variable, which is represented in this documentation by a hash character (#). In USX the attribute number indicates:

	* A portion of a complete element, or relative weighting of the "pieces" of the elements, such as \mt1, \mt2, \mt3 which are all parts of a major title.
	* The level of division (hierarchy).
	* The level of indentation relative to other like elements, as in poetry (q#) or lists (li#) or outlines (io#).
	
	**style = style1** — The unnumbered version of a style attribute may be used when only one level of this paragraph style exists within the project text. Numbers should always be included when more than one level of the paragraph style exists within the project text.

.. index:: usx <para> (identification)
.. _usx-parastyles_identification:

Identification
--------------
* ide
* rem
* :ref:`h <usx-parastyle_h>`
* :ref:`toc1 <usx-parastyle_toc1>`
* :ref:`toc2 <usx-parastyle_toc2>`
* :ref:`toc3 <usx-parastyle_toc3>`

-----


.. _usx-parastyle_h:
.. index:: para @style (h)

:@style: h
:Use: Running header text.
:Valid In: :ref:`usx-div_bookHeader`

	.. image:: images/usx-para-style_h.jpg
		:width: 300px

-----

.. _usx-parastyle_toc1:
.. index:: para @style (toc1)

:@style: toc1
:Use: Long table of contents text.
:Valid In: :ref:`usx-div_bookHeader`

-----

.. _usx-parastyle_toc2:
.. index:: para @style (toc2)

:@style: toc2
:Use: Short table of contents text.
:Valid In: :ref:`usx-div_bookHeader`

-----

.. _usx-parastyle_toc3:
.. index:: para @style (toc3)

:@style: toc3
:Use: Book abbreviation.
:Valid In: :ref:`usx-div_bookHeader`

-----

.. note:: **About toc1, toc2, toc3**

	The `metadata.xml <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/metadata.html>`_ file within a DBL `text release bundle <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/index.html>`_ contains a `bookNames <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/metadata.html#booknames>`_ element in which each scripture book is itemized together with child elements for its long, short and abbreviated forms. The `bookNames <http://app.thedigitalbiblelibrary.org/static/docs/entryref/text/metadata.html#booknames>`_ element is the key location where this book naming metadata is contained within the bundle. USX para elements with attributes toc1, toc2, or toc3 are strictly optional data. Their presence in a USX file is valid, but reflects a legacy form of USFM markup in which the USFM files for each book were the key location for this book naming metadata.

.. index:: usx <para> (introductions)
.. _usx-parastyles_introductions:

Introductions
-------------
* :ref:`imt# <usx-parastyle_imt>`
* :ref:`is# <usx-parastyle_is>`
* :ref:`ip <usx-parastyle_ip>`
* :ref:`ipi <usx-parastyle_ipi>`
* :ref:`im <usx-parastyle_im>`
* :ref:`imi <usx-parastyle_imi>`
* :ref:`ipq <usx-parastyle_ipq>`
* :ref:`imq <usx-parastyle_imq>`
* :ref:`ipr <usx-parastyle_ipr>`
* :ref:`iq <usx-parastyle_iq>`
* :ref:`ib <usx-parastyle_ib>`
* :ref:`ili# <usx-parastyle_ili>`
* :ref:`iot <usx-parastyle_iot>`
* :ref:`io# <usx-parastyle_io>`
* :ref:`iex <usx-parastyle_iex>`
* :ref:`imte# <usx-parastyle_imte>`
* :ref:`ie <usx-parastyle_ie>`

-----

.. _usx-parastyle_imt:
.. index:: para @style (imt)

:@style: imt#
:Use: Introduction major title. |br|
	# denotes the title level or relative weighting. |br|
	**imt = imt1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_imt.jpg
		:width: 250px

-----

.. _usx-parastyle_is:
.. index:: para @style (is)

:@style: is#
:Use: Introduction section heading. |br|
	# denotes the title level or relative weighting. |br|
	**is = is1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_is.jpg
		:width: 250px

-----

.. _usx-parastyle_ip:
.. index:: para @style (ip)

:@style: ip
:Use: Introduction paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_ip.jpg
		:width: 250px

-----

.. _usx-parastyle_ipi:
.. index:: para @style (ipi)

:@style: ipi
:Use: Indented introduction paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_ipi.jpg
		:width: 250px

-----

.. _usx-parastyle_im:
.. index:: para @style (im)

:@style: im
:Use: Introduction flush left (margin) paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_im.jpg
		:width: 250px

-----

.. _usx-parastyle_imi:
.. index:: para @style (imi)

:@style: imi
:Use: Indented introduction flush left (margin) paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_imi.jpg
		:width: 250px

-----

.. _usx-parastyle_ipq:
.. index:: para @style (ipq)

:@style: ipq
:Use: Introduction quote from scripture text paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_ipq.jpg
		:width: 300px

-----

.. _usx-parastyle_imq:
.. index:: para @style (imq)

:@style: imq
:Use: Introduction flush left (margin) quote from scripture text paragraph.
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_imq.jpg
		:width: 300px

-----

.. _usx-parastyle_ipr:
.. index:: para @style (ipr)

:@style: ipr
:Use: Introduction right-aligned paragraph. |br|
	Typically used for the reference for a quote from the scripture text (:ref:`imq <usx-parastyle_imq>`, :ref:`ipq <usx-parastyle_ipq>`)
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_ipr.jpg
		:width: 250px

-----

.. _usx-parastyle_iq:
.. index:: para @style (iq)

:@style: iq#
:Use: Introduction poetic line. |br|
	# represents the level of indent (i.e. \iq1, \iq2, \iq3 etc.) |br|
	**iq = iq1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_iq.jpg
		:width: 250px

-----

.. _usx-parastyle_ib:
.. index:: para @style (ib)

:@style: ib
:Use: Introduction blank line. |br|
	May be used to explicitly indicate additional white space between paragraphs.
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_ili:
.. index:: para @style (ili)

:@style: ili#
:Use: Introduction list item. |br|
	# represents the level of indent |br|
	**ili = ili1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_ili.jpg
		:width: 250px

-----

.. _usx-parastyle_iot:
.. index:: para @style (iot)

:@style: iot
:Use: Introduction outline title. (see :ref:`io# <usx-parastyle_io>` below)
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_io:
.. index:: para @style (io)

:@style: io#
:Use: Introduction outline entry. |br|
	The outline entry typically ends with a range of references in parentheses. |br|
	References may be marked with char @style :ref:`ior <usx-charstyle_ior>`. |br|
	# represents the outline (indent) level.
	**io = io1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

	.. image:: images/usx-para-style_io.jpg
		:width: 300px

-----

:@style: :ref:`ior <usx-charstyle_ior>`
:See: :doc:`char <charstyles>` @style :ref:`ior <usx-charstyle_ior>`

-----

.. _usx-parastyle_iex:
.. index:: para @style (iex)

:@style: iex
:Use: Introduction explanatory or bridge text (e.g. explanation of missing book in a short Old Testament). |br|
	*This para @style is used within Chapter Text.*
:Valid In: :ref:`usx-div_bookIntroduction`

-----

:@style: :ref:`iqt <usx-charstyle_iqt>`
:See: :doc:`char <charstyles>` @style :ref:`iqt <usx-charstyle_iqt>`

-----

.. _usx-parastyle_imte:
.. index:: para @style (imte)

:@style: imt#
:Use: Introduction major title ending. |br|
	Used to mark a major title indicating the end of the introduction. |br|
	# represents a portion of the title, with the lesser emphasis (relative weighting) being on the higher numbers. |br|
	**imte = imte1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_ie:
.. index:: para @style (ie)

:@style: ie
:Use: Introduction end. |br|
	Optionally included to explicitly indicate the end of the introduction material.
:Valid In: :ref:`usx-div_bookIntroduction`

.. index:: usx <para> (titles & headings)
.. _usx-parastyles_titles_headings:

Titles and Headings
-------------------
* :ref:`mt# <usx-parastyle_mt>`
* :ref:`mte# <usx-parastyle_mte>`
* :ref:`ms# <usx-parastyle_ms>`
* :ref:`mr <usx-parastyle_mr>`
* :ref:`s# <usx-parastyle_s>`
* :ref:`sr <usx-parastyle_sr>`
* :ref:`r <usx-parastyle_r>`
* :ref:`d <usx-parastyle_d>`
* :ref:`sp <usx-parastyle_sp>`

-----

.. _usx-parastyle_mt:
.. index:: para @style (mt)

:@style: mt#
:Use: Main title. |br|
	Key components in the title of a biblical book. |br|
	# represents a portion of the title, with the lesser emphasis (relative weighting) being on the higher numbers. |br|
	**mt = mt1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_bookTitles`

	.. image:: images/usx-para-style_mt.jpg
		:width: 250px

	|br|

	.. image:: images/usx-para-style_mtAlt.jpg
		:width: 250px

-----

.. _usx-parastyle_mte:
.. index:: para @style (mte)

:@style: mte#
:Use: Main title at introduction ending. |br|
	May be used in texts which repeat the main title at the end of the introduction.
:Valid In: :ref:`usx-div_bookIntroduction`

-----

.. _usx-parastyle_ms:
.. index:: para @style (ms)

:@style: ms#
:Use: Major section heading.
	A heading added before a broader text division than what is typically considered a "section" division (see :ref:`s# <usx-parastyle_s>`). |br|
	# represents the level of division. |br|
	**ms = ms1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_ms.jpg
		:width: 250px

	|br|

	.. image:: images/usx-para-style_msAlt.jpg
		:width: 250px

-----

.. _usx-parastyle_mr:
.. index:: para @style (mr)

:@style: mr
:Use: Major section reference range. |br|
	The text reference range listed under a major section heading.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_mr.jpg
		:width: 250px

-----

.. _usx-parastyle_s:
.. index:: para @style (s)

:@style: s#
:Use: Section heading. |br|
	The typical (common) section division heading. |br|
	# represents the level of division. |br|
	**s = s1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapterText`
	
	*s1 example*

	.. image:: images/usx-para-style_s1.jpg
		:width: 250px

	|br| *s2 example*

	.. image:: images/usx-para-style_s2.jpg
		:width: 250px

-----

.. _usx-parastyle_sr:
.. index:: para @style (sr)

:@style: sr
:Use: Section reference range. |br|
	The text reference range listed under a section heading. |br|
	sr is not equivalent to r which is used for marking parallel references. |br|
:See also: :ref:`mr <usx-parastyle_mr>`
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_sr.jpg
		:width: 250px

-----

.. _usx-parastyle_r:
.. index:: para @style (r)

:@style: r
:Use: Parallel passage reference(s). |br|
	A reference to a parallel passage usually located under a section heading :ref:`s# <usx-parastyle_s>`. |br|
:See also: :doc:`char <charstyles>` @style :ref:`rq <usx-charstyle_rq>`.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_r.jpg
		:width: 250px

-----

.. _usx-parastyle_d:
.. index:: para @style (d)

:@style: d
:Use: Descriptive title (or "Hebrew subtitle"). |br|
	Sometimes used in Psalms under the section title (e.g. "For the director of Music").
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_d.jpg
		:width: 250px

-----

.. _usx-parastyle_sp:
.. index:: para @style (sp)

:@style: sp
:Use: Speaker identification (e.g. Job and Song of Songs).
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_sp.jpg
		:width: 250px

.. index:: usx <para> (paragraphs)
.. _usx-parastyles_paragraphs:

Paragraphs
----------
* :ref:`p <usx-parastyle_p>`
* :ref:`m <usx-parastyle_m>`
* :ref:`pmo <usx-parastyle_pmo>`
* :ref:`pm <usx-parastyle_pm>`
* :ref:`pmc <usx-parastyle_pmc>`
* :ref:`pmr <usx-parastyle_pmr>`
* :ref:`pi# <usx-parastyle_pi>`
* :ref:`mi <usx-parastyle_mi>`
* :ref:`cls <usx-parastyle_cls>`
* :ref:`li# <usx-parastyle_li>`
* :ref:`pc <usx-parastyle_pc>`
* :ref:`pr <usx-parastyle_pr>`
* :ref:`ph# <usx-parastyle_ph>`
* :ref:`lit <usx-parastyle_lit>`

-----

.. _usx-parastyle_p:
.. index:: para @style (p)

:@style: p
:Use: Normal paragraph.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_p.jpg
		:width: 250px

-----

.. _usx-parastyle_m:
.. index:: para @style (m)

:@style: m
:Use: Margin paragraph. |br|
	Typically used to resume prose at the margin (without indent) after poetry or OT quotation (i.e. a continuation of the previous paragraph).
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_m.jpg
		:width: 250px

-----

.. _usx-parastyle_pmo:
.. index:: para @style (pmo)

:@style: pmo
:Use: Embedded text opening.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_pmo.jpg
		:width: 250px

-----

.. _usx-parastyle_pm:
.. index:: para @style (pm)

:@style: pm
:Use: Embedded text paragraph.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_pm.jpg
		:width: 250px

-----

.. _usx-parastyle_pmc:
.. index:: para @style (pmc)

:@style: pmc
:Use: Embedded text closing.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_pmc.jpg
		:width: 250px

-----

.. _usx-parastyle_pmr:
.. index:: para @style (pmr)

:@style: pmr
:Use: Embedded text refrain.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_pmr.jpg
		:width: 250px

-----

.. _usx-parastyle_pi:
.. index:: para @style (pi)

:@style: pi#
:Use: Indented paragraph. |br|
	Used in some texts for discourse sections. |br|
	# represents the level of indent. |br|
	**pi = pi1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:See also: :ref:`pm <usx-parastyle_pm>`
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_pi.jpg
		:width: 250px

-----

.. _usx-parastyle_mi:
.. index:: para @style (mi)

:@style: mi
:Use: Indented flush left paragraph
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_mi.jpg
		:width: 250px

-----

.. _usx-parastyle_cls:
.. index:: para @style (cls)

:@style: cls
:Use: Closure of an epistle / letter
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_cls.jpg
		:width: 250px

-----

.. _usx-parastyle_li:
.. index:: para @style (li)

:@style: li#
:Use: List item (out-dented paragraph meant to highlight the items of a list.). |br|
	# represents the level of indent |br|
	**li = li1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_li.jpg
		:width: 250px

-----

.. _usx-parastyle_pc:
.. index:: para @style (pc)

:@style: pc
:Use: Centered paragraph
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_pc.jpg
		:width: 250px

-----

.. _usx-parastyle_pr:
.. index:: para @style (pr)

:@style: pr
:Use: Right-aligned paragraph |br| |br|
	|ico_W| Use is strongly discouraged. |br|
	|ico_Cg| Recommended alternate is :ref:`pmr <usx-parastyle_pmr>` |br|
:Valid In: :ref:`usx-div_chapterText`

-----

.. _usx-parastyle_ph:
.. index:: para @style (ph)

:@style: ph#
:Use: Indented paragraph with hanging indent. |br|
	# represents the level of indent |br|
	**ph = ph1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes) |br| |br|
	|ico_W| Use is strongly discouraged. |br|
	|ico_Cg| Recommended alternate is :ref:`li# <usx-parastyle_li>` |br|
:Valid In: :ref:`usx-div_chapterText`

-----

.. _usx-parastyle_lit:
.. index:: para @style (lit)

:@style: lit
:Use: Liturgical note/comment. (e.g. a guide which tells the reader/worshiper that he/she should recite a prayer or recitation etc.) |br|
	*In the formatting example image (below) the word Слава = "Glory"*
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_lit.jpg
		:width: 250px

.. index:: usx <para> (poetry)
.. _usx-parastyles_poetry:

Poetry
------
* :ref:`q# <usx-parastyle_q>`
* :ref:`qr <usx-parastyle_qr>`
* :ref:`qc <usx-parastyle_qc>`
* :ref:`qa <usx-parastyle_qa>`
* :ref:`qm# <usx-parastyle_qm>`
* :ref:`b <usx-parastyle_b>`

-----

.. _usx-parastyle_q:
.. index:: para @style (q)

:@style: q#
:Use: Poetic line. |br|
	# represents the level of indent (i.e. \q1, \q2, \q3 etc.).
	**q = q1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_q1.jpg
		:width: 250px

	|br|

	.. image:: images/usx-para-style_q2.jpg
		:width: 250px

-----

.. _usx-parastyle_qr:
.. index:: para @style (qr)

:@style: qr
:Use: Right-aligned poetic line. |br|
	|ico_Cg| Common use: Poetic refrain
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_qr.jpg
		:width: 250px

-----

.. _usx-parastyle_qc:
.. index:: para @style (qc)

:@style: qc
:Use: Centered poetic line.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_qc.jpg
		:width: 250px

-----

.. _usx-parastyle_qa:
.. index:: para @style (qa)

:@style: qa
:Use: Acrostic heading.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_qa.jpg
		:width: 250px

-----

:@style: :ref:`qac <usx-charstyle_qac>`
:See: :doc:`char <charstyles>` @style :ref:`qac <usx-charstyle_qac>`

-----

.. _usx-parastyle_qm:
.. index:: para @style (qm)

:@style: qm#
:Use: Embedded text poetic line. |br|
	# represents the level of indent (i.e. \qm1, \qm2, etc.). |br|
	**qm = qm1** (see :ref:`notes <usx-notes_numberedStyles>` on numbered @style attributes)
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_qm.jpg
		:width: 250px

-----

:@style: :ref:`qs <usx-charstyle_qs>`
:See: :doc:`char <charstyles>` @style :ref:`qs <usx-charstyle_qs>`

-----

.. _usx-parastyle_b:
.. index:: para @style (b)

:@style: b
:Use: Blank line. |br|
	May be used to explicitly indicate additional white space between paragraphs. |br| |br|
	|ico_W| A para element with **b** style type should always be *empty*. |br|
	**b** should not be used before or after titles to indicate white-space.
:Valid In: :ref:`usx-div_chapterText`

	.. image:: images/usx-para-style_b.jpg
		:width: 250px

	|br|

	.. image:: images/usx-para-style_bAlt.jpg
		:width: 250px
