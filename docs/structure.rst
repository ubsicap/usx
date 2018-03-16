.. include:: /_static/inc_styles.txt

.. _usx_docStructure:

Document Structure
==================

A USX document consists of valid elements for either :ref:`Scripture <usx-type_scripture>` or :ref:`Peripheral <usx-type_peripheral>` types organized within a sequence of document divisions.

.. image:: images/usx_USX.png

-----

.. index:: document type; scripture
.. _usx-type_scripture:

Scripture
---------

.. image:: images/usx-type_Scripture.png

* :ref:`Book Identification<usx-div_bookIdentification>` |req|
* :ref:`Book Headers<usx-div_bookHeaders>`
* :ref:`Book Titles<usx-div_bookTitles>` |req| +
* :ref:`Book Introduction<usx-div_bookIntroduction>`
* :ref:`Book Introduction End Titles<usx-div_bookIntroductionEndTitles>`
* :ref:`Book Chapter Label<usx-div_bookChapterLabel>`
* :ref:`Chapter Content<usx-div_chapterContent>` |req| +

|req| = *required* ; + = *one or more*

-----

.. index:: document type; peripheral
.. _usx-type_peripheral:

Peripheral
----------

|badge_3.0|

A USX document containing peripheral content will be either:

* a document containing content for a :ref:`single peripheral book <usx-type_peripheralBook>` (:ref:`Concordance <usx-book_CNC>`, :ref:`Glossary <usx-book_GLO>`, :ref:`Topical Index <usx-book_GLO>`, :ref:`Names Index <usx-book_TDX>`), or
* a document containing content for a :ref:`division (sub-section) of peripheral content <usx-type_peripheralBookSection>` from a larger book (:doc:`Front Matter <peripherals/front>`, :doc:`Introductions <peripherals/intros>`, :doc:`Back Matter <peripherals/back>`, :doc:`Other <peripherals/other>`)

|ico_See| *See:* :doc:`Peripherals <peripherals>` for additional information on peripheral content organization. 

.. image:: images/usx-type_Peripheral.png

.. index:: document type; peripheral book
.. _usx-type_peripheralBook:

Peripheral Book
^^^^^^^^^^^^^^^

.. image:: images/usx-type_PeripheralBook.png

* :ref:`Book Identification <usx-div_bookIdentification>` |req|
* :ref:`Book Headers<usx-div_bookHeaders>`
* :ref:`Book Titles<usx-div_bookTitles>` |req| +
* :ref:`Book Introduction<usx-div_bookIntroduction>`
* :ref:`Book Introduction End Titles<usx-div_bookIntroductionEndTitles>`
* :ref:`Book Chapter Label<usx-div_bookChapterLabel>`
* :ref:`Peripheral Content<usx-div_peripheralContent>` |req| +

.. index:: document type; peripheral book section
.. _usx-type_peripheralBookSection:

Peripheral Book Section
^^^^^^^^^^^^^^^^^^^^^^^

.. image:: images/usx-type_PeripheralBookSection.png

* :ref:`Book Identification <usx-div_bookIdentification>` |req|
* :ref:`<periph> <usx-element_periph>` Element |req|

    * :ref:`Book Headers<usx-div_bookHeaders>`
    * :ref:`Book Titles<usx-div_bookTitles>` |req| +
    * :ref:`Book Introduction<usx-div_bookIntroduction>`
    * :ref:`Book Introduction End Titles<usx-div_bookIntroductionEndTitles>`
    * :ref:`Book Chapter Label<usx-div_bookChapterLabel>`
    * :ref:`Peripheral Content<usx-div_peripheralContent>` |req| +

|req| = *required* ; + = *one or more*

-----

.. index:: document structure; book identification
.. _usx-div_bookIdentification:

Book Identification
-------------------

.. image:: images/usx-div_BookIdentification.png

The :ref:`book <usx-element_book>` element for primary book identification.

-----

.. index:: document structure; book headers
.. _usx-div_bookHeaders:

Book Headers
------------

.. image:: images/usx-div_BookHeaders.png

An optional collection of one or more :ref:`para <usx-element_para>` elements for providing vernacular book name and abbreviation texts.

* Valid @style types (alphabetical): :ref:`h <usx-parastyle_h>`, ide, rem, :ref:`toc1 <usx-parastyle_toc1>`, :ref:`toc2 <usx-parastyle_toc2>`, :ref:`toc3 <usx-parastyle_toc3>`

-----

.. index:: document structure; book titles
.. _usx-div_bookTitles:

Book Titles
-----------

.. image:: images/usx-div_BookTitles.png

A collection of one or more :ref:`para <usx-element_para>` elements for book main titles.

* Valid @style types (alphabetical): :ref:`imt <usx-parastyle_imt>`, :ref:`imt1 <usx-parastyle_imt>`, :ref:`imt2 <usx-parastyle_imt>`, :ref:`mt <usx-parastyle_mt>`, :ref:`mt1 <usx-parastyle_mt>`, :ref:`mt2 <usx-parastyle_mt>`, :ref:`mt3 <usx-parastyle_mt>`, :ref:`mt4 <usx-parastyle_mt>`, rem
* Optional collection of one or more child elements (may be nested): :ref:`note <usx-element_note>` (@style f, fe, x), :ref:`char <usx-element_char>`, :ref:`optbreak <usx-element_optbreak>`

-----

.. index:: document structure; book introduction
.. _usx-div_bookIntroduction:

Book Introduction
-----------------

.. image:: images/usx-div_BookIntroduction.png

An optional collection of :ref:`para <usx-element_para>` or :ref:`table <usx-element_table>` elements for book introductions.

* Valid @style types (alphabetical): :ref:`ib <usx-parastyle_ib>`, :ref:`ie <usx-parastyle_ie>`, :ref:`iex <usx-parastyle_iex>`, :ref:`ili <usx-parastyle_ili>`, :ref:`ili1 <usx-parastyle_ili>`, :ref:`ili2 <usx-parastyle_ili>`, :ref:`im <usx-parastyle_im>`, :ref:`imi <usx-parastyle_im>`, :ref:`imq <usx-parastyle_imq>`, :ref:`imt <usx-parastyle_imt>`, :ref:`imt1 <usx-parastyle_imt>`, :ref:`imt2 <usx-parastyle_imt>`, :ref:`imt3 <usx-parastyle_imt>`, :ref:`imt4 <usx-parastyle_imt>`, :ref:`imte <usx-parastyle_imte>`, :ref:`imte1 <usx-parastyle_imte>`, :ref:`imte2 <usx-parastyle_imte>`, :ref:`io <usx-parastyle_io>`, :ref:`io1 <usx-parastyle_io>`, :ref:`io2 <usx-parastyle_io>`, :ref:`io3 <usx-parastyle_io>`, :ref:`io4 <usx-parastyle_io>`, :ref:`iot <usx-parastyle_iot>`, :ref:`ip <usx-parastyle_ip>`, :ref:`ipi <usx-parastyle_ipi>`, :ref:`ipq <usx-parastyle_ipq>`, :ref:`ipr <usx-parastyle_ipr>`, :ref:`iq <usx-parastyle_iq>`, :ref:`iq1 <usx-parastyle_iq>`, :ref:`iq2 <usx-parastyle_iq>`, :ref:`iq3 <usx-parastyle_iq>`, :ref:`is <usx-parastyle_is>`, :ref:`is1 <usx-parastyle_is>`, :ref:`is2 <usx-parastyle_is>`, rem
* Optional collection of one or more child elements: :ref:`note <usx-element_note>` (@style f, fe, x), :ref:`ref <usx-element_ref>`, :ref:`char <usx-element_char>`, :ref:`ms <usx-element_ms>`, :ref:`figure <usx-element_figure>`

-----

.. index:: document structure; book introduction end titles
.. _usx-div_bookIntroductionEndTitles:

Book Introduction End Titles
----------------------------

.. image:: images/usx-div_BookIntroductionEndTitles.png

An optional collection of :ref:`para <usx-element_para>` elements for book titles occurring at the end of the book introduction.

* Valid @style types (alphabetical): :ref:`imt <usx-parastyle_imt>`, :ref:`imt1 <usx-parastyle_imt>`, :ref:`imt2 <usx-parastyle_imt>`, :ref:`mt <usx-parastyle_mt>`, :ref:`mt1 <usx-parastyle_mt>`, :ref:`mt2 <usx-parastyle_mt>`, :ref:`mt3 <usx-parastyle_mt>`, :ref:`mt4 <usx-parastyle_mt>`
* Optional collection of one or more child elements: :ref:`note <usx-element_note>` (@style f, fe, x), :ref:`ref <usx-element_ref>`, :ref:`char <usx-element_char>`, :ref:`ms <usx-element_ms>`, :ref:`optbreak <usx-element_optbreak>`

-----

.. index:: document structure; book chapter label
.. _usx-div_bookChapterLabel:

Book Chapter Label
------------------

.. image:: images/usx-div_BookChapterLabel.png

An optional :ref:`para <usx-element_para>` element for a chapter heading text which could be applied (typically as a heading) to all chapters in the current book.

* Valid @style types: :ref:`cl <usx-parastyle_cl>`

-----

.. index:: document structure; chapter
.. _usx-div_chapterContent:

Chapter Content
---------------

.. image:: images/usx-div_ChapterContent.png

An optional collection of :ref:`chapter <usx-element_chapter>`, :ref:`para <usx-element_para>`, :ref:`table <usx-element_table>`, or :ref:`sidebar <usx-element_sidebar>` elements for the main content of a scripture book.

* Valid :ref:`para <usx-element_para>` @style types (alphabetical): :ref:`imt1 <usx-parastyle_imt>`, :ref:`b <usx-parastyle_b>`, :ref:`cd <usx-parastyle_cd>`, :ref:`cl <usx-parastyle_cl>`, :ref:`cls <usx-parastyle_cls>`, cp, :ref:`d <usx-parastyle_d>`, :ref:`iex <usx-parastyle_iex>`, :ref:`ip <usx-parastyle_ip>`, k1, k2, :ref:`lf <usx-parastyle_lf>`, :ref:`lh <usx-parastyle_lh>`, :ref:`li <usx-parastyle_li>`, :ref:`li1 <usx-parastyle_li>`, :ref:`li2 <usx-parastyle_li>`, :ref:`li3 <usx-parastyle_li>`, :ref:`li4 <usx-parastyle_li>`, :ref:`lim <usx-parastyle_lim>`, :ref:`lim1 <usx-parastyle_lim>`, :ref:`lim2 <usx-parastyle_lim>`, :ref:`lim3 <usx-parastyle_lim>`, :ref:`lim4 <usx-parastyle_lim>`, :ref:`lit <usx-parastyle_lit>`, :ref:`m <usx-parastyle_m>`, :ref:`mi <usx-parastyle_mi>`, :ref:`mr <usx-parastyle_mr>`, :ref:`ms <usx-parastyle_ms>`, :ref:`ms1 <usx-parastyle_ms>`, :ref:`ms2 <usx-parastyle_ms>`, :ref:`ms3 <usx-parastyle_ms>`, :ref:`mte <usx-parastyle_mte>`, :ref:`mte1 <usx-parastyle_mte>`, :ref:`mte2 <usx-parastyle_mte>`, :ref:`p <usx-parastyle_p>`, :ref:`p <usx-parastyle_p>`, :ref:`p1 <usx-parastyle_p>`, :ref:`p2 <usx-parastyle_p>`, :ref:`pc <usx-parastyle_pc>`, :ref:`pi <usx-parastyle_pi>`, :ref:`pi1 <usx-parastyle_pi>`, :ref:`pi2 <usx-parastyle_pi>`, :ref:`pi3 <usx-parastyle_pi>`, :ref:`pm <usx-parastyle_pm>`, :ref:`pmc <usx-parastyle_pmc>`, :ref:`pmo <usx-parastyle_pmo>`, :ref:`pmr <usx-parastyle_pmr>`, :ref:`po <usx-parastyle_po>`, :ref:`q <usx-parastyle_q>`, :ref:`q1 <usx-parastyle_q>`, :ref:`q2 <usx-parastyle_q>`, :ref:`q3 <usx-parastyle_q>`, :ref:`q4 <usx-parastyle_q>`, :ref:`qa <usx-parastyle_qa>`, :ref:`qc <usx-parastyle_qc>`, :ref:`qd <usx-parastyle_qd>`, :ref:`qm <usx-parastyle_qm>`, :ref:`qm1 <usx-parastyle_qm>`, :ref:`qm2 <usx-parastyle_qm>`, :ref:`qm3 <usx-parastyle_qm>`, :ref:`qr <usx-parastyle_qr>`, :ref:`r <usx-parastyle_r>`, rem, restore, :ref:`s <usx-parastyle_s>`, :ref:`s1 <usx-parastyle_s>`, :ref:`s2 <usx-parastyle_s>`, :ref:`s3 <usx-parastyle_s>`, :ref:`s4 <usx-parastyle_s>`, :ref:`sd <usx-parastyle_sd>`, :ref:`sd1 <usx-parastyle_sd>`, :ref:`sd2 <usx-parastyle_sd>`, :ref:`sd3 <usx-parastyle_sd>`, :ref:`sd4 <usx-parastyle_sd>`, :ref:`sp <usx-parastyle_sp>`, :ref:`sr <usx-parastyle_sr>`

* Optional collection of one or more child elements: :ref:`note <usx-element_note>` (@style f, fe, ef, x, ex), :ref:`ref <usx-element_ref>`, :ref:`char <usx-element_char>`, :ref:`ms <usx-element_ms>`, :ref:`figure <usx-element_figure>`, :ref:`verse <usx-element_verse>`, :ref:`optbreak <usx-element_optbreak>`

-----

.. _usx-div_peripheralContent:

Peripheral Content
------------------

.. image:: images/usx-div_PeripheralContent.png

An optional collection of :ref:`chapter <usx-element_chapter>`, :ref:`para <usx-element_para>`, :ref:`table <usx-element_table>`, or :ref:`sidebar <usx-element_sidebar>` elements for the main content of a scripture book.

* Valid :ref:`para <usx-element_para>` @style types (alphabetical): :ref:`imt1 <usx-parastyle_imt>`, :ref:`b <usx-parastyle_b>`, :ref:`cd <usx-parastyle_cd>`, :ref:`cl <usx-parastyle_cl>`, :ref:`cls <usx-parastyle_cls>`, cp, :ref:`d <usx-parastyle_d>`, :ref:`iex <usx-parastyle_iex>`, :ref:`ip <usx-parastyle_ip>`, k1, k2, :ref:`lf <usx-parastyle_lf>`, :ref:`lh <usx-parastyle_lh>`, :ref:`li <usx-parastyle_li>`, :ref:`li1 <usx-parastyle_li>`, :ref:`li2 <usx-parastyle_li>`, :ref:`li3 <usx-parastyle_li>`, :ref:`li4 <usx-parastyle_li>`, :ref:`lim <usx-parastyle_lim>`, :ref:`lim1 <usx-parastyle_lim>`, :ref:`lim2 <usx-parastyle_lim>`, :ref:`lim3 <usx-parastyle_lim>`, :ref:`lim4 <usx-parastyle_lim>`, :ref:`lit <usx-parastyle_lit>`, :ref:`m <usx-parastyle_m>`, :ref:`mi <usx-parastyle_mi>`, :ref:`mr <usx-parastyle_mr>`, :ref:`ms <usx-parastyle_ms>`, :ref:`ms1 <usx-parastyle_ms>`, :ref:`ms2 <usx-parastyle_ms>`, :ref:`ms3 <usx-parastyle_ms>`, :ref:`mte <usx-parastyle_mte>`, :ref:`mte1 <usx-parastyle_mte>`, :ref:`mte2 <usx-parastyle_mte>`, :ref:`p <usx-parastyle_p>`, :ref:`p <usx-parastyle_p>`, :ref:`p1 <usx-parastyle_p>`, :ref:`p2 <usx-parastyle_p>`, :ref:`pc <usx-parastyle_pc>`, :ref:`pi <usx-parastyle_pi>`, :ref:`pi1 <usx-parastyle_pi>`, :ref:`pi2 <usx-parastyle_pi>`, :ref:`pi3 <usx-parastyle_pi>`, :ref:`pm <usx-parastyle_pm>`, :ref:`pmc <usx-parastyle_pmc>`, :ref:`pmo <usx-parastyle_pmo>`, :ref:`pmr <usx-parastyle_pmr>`, :ref:`po <usx-parastyle_po>`, :ref:`q <usx-parastyle_q>`, :ref:`q1 <usx-parastyle_q>`, :ref:`q2 <usx-parastyle_q>`, :ref:`q3 <usx-parastyle_q>`, :ref:`q4 <usx-parastyle_q>`, :ref:`qa <usx-parastyle_qa>`, :ref:`qc <usx-parastyle_qc>`, :ref:`qd <usx-parastyle_qd>`, :ref:`qm <usx-parastyle_qm>`, :ref:`qm1 <usx-parastyle_qm>`, :ref:`qm2 <usx-parastyle_qm>`, :ref:`qm3 <usx-parastyle_qm>`, :ref:`qr <usx-parastyle_qr>`, :ref:`r <usx-parastyle_r>`, rem, restore, :ref:`s <usx-parastyle_s>`, :ref:`s1 <usx-parastyle_s>`, :ref:`s2 <usx-parastyle_s>`, :ref:`s3 <usx-parastyle_s>`, :ref:`s4 <usx-parastyle_s>`, :ref:`sd <usx-parastyle_sd>`, :ref:`sd1 <usx-parastyle_sd>`, :ref:`sd2 <usx-parastyle_sd>`, :ref:`sd3 <usx-parastyle_sd>`, :ref:`sd4 <usx-parastyle_sd>`, :ref:`sp <usx-parastyle_sp>`, :ref:`sr <usx-parastyle_sr>`

* Optional collection of one or more child elements: :ref:`note <usx-element_note>` (@style f, fe, ef, x, ex), :ref:`ref <usx-element_ref>`, :ref:`char <usx-element_char>`, :ref:`ms <usx-element_ms>`, :ref:`figure <usx-element_figure>`, :ref:`verse <usx-element_verse>`, :ref:`optbreak <usx-element_optbreak>`