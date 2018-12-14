.. include:: /_static/inc_styles.txt

.. index:: release notes

Release Notes
=============

.. _about_release_3.0:

3.0
^^^

USX 3.0 additions or revisions are highlighted throughout this documentation using the badge |badge_3.0|

*April 2018*

**Element / Attribute Additions**

* Letter opening: :ref:`<para> <usx-element_para>` @style :ref:`po <usx-parastyle_po>`
* List header and footer elements: :ref:`<para> <usx-element_para>` @style :ref:`lh <usx-parastyle_lh>` and :ref:`lf <usx-parastyle_lf>`
* Embedded list: :ref:`<para> <usx-element_para>` @style :ref:`lim# <usx-parastyle_lim>`
* Hebrew note: :ref:`<para> <usx-element_para>` @style :ref:`qd <usx-parastyle_qd>`
* Semantic division: :ref:`<para> <usx-element_para>` @style :ref:`sd# <usx-parastyle_sd>`
* Aramaic wordlist entry: :ref:`<char> <usx-element_char>` @style :ref:`wa <usx-charstyle_wa>`
* Geographic proper name (Chinese texts): :ref:`<char> <usx-element_char>` @style :ref:`png <usx-charstyle_png>`
* Target references “added” text: :ref:`<char> <usx-element_char>` @style :ref:`xta <usx-note_crossReference_charstyle_xta>`
* Published cross reference origin text: :ref:`<char> <usx-element_char>` @style :ref:`xop <usx-note_crossReference_charstyle_xop>`
* Structured list items: :ref:`<char> <usx-element_char>` @style :ref:`lik <usx-charstyle_lik>` and :ref:`liv# <usx-charstyle_liv>`
* List item total: :ref:`<char> <usx-element_char>` @style :ref:`litl <usx-charstyle_litl>`
* Link text: :ref:`<char> <usx-element_char>` @style :ref:`jmp <usx-charstyle_jmp>`
* Ruby glosses (CJK texts): :ref:`<char> <usx-element_char>` @style :ref:`rb <usx-charstyle_rb>`
* Milestone element: :ref:`<ms> <usx-element_ms>`

    * :doc:`Milestone @style types </msstyles>` for quotations: :ref:`qt#-s and qt#-e <usx-msstyle_qt>`
    
        - Add :doc:`attribute </attributes>` ``who`` for :ref:`qt#-s and qt#-e <usx-msstyle_qt-attr>`
    
    * :doc:`Milestone @style types </msstyles>` for translators sections: :ref:`ts-s and ts-e <usx-msstyle_ts>`

* :ref:`<char> <usx-element_char>` @style types providing additional attributes

    * :ref:`<char> <usx-element_char>` @style :ref:`w <usx-charstyle_w-attr>` (``lemma``, ``strong``, ``scrloc``)
    * :ref:`<char> <usx-element_char>` @style :ref:`rb <usx-charstyle_rb-attr>` (``gloss``)

* Verse start ``sid`` and end ``eid`` identifier :doc:`attributes </attributes>` for :ref:`<verse> <usx-element_verse>`.
* Verse identifier ``vid`` :doc:`attribute </attributes>` for :ref:`<para> <usx-element_para>`.
* Strategy for applying USX markup to project :doc:`peripheral contents </peripherals>`.
* Standard :ref:`peripheral identifiers <usx-vocab-peripheralIds>`.

**Element / Attribute Revisions**

* Require a :ref:`<chapter> <usx-element_chapter>` milestone at start and end of chapter text.

    * Chapter start ``sid`` and end ``eid`` identifier :doc:`attributes </attributes>` for :ref:`<chapter> <usx-element_chapter>`.

* Require a :ref:`<verse> <usx-element_verse>` milestone at start and end of verse text.

    * Verse start ``sid`` and end ``eid`` identifier :doc:`attributes </attributes>` for :ref:`<verse> <usx-element_verse>`.

* Require a verse identifier ``vid`` :doc:`attribute </attributes>` for :ref:`<para> <usx-element_para>` to re-identify the current verse whenever the previous :ref:`para <usx-element_para>` or :ref:`table <usx-element_table>` closed prior the end of the current verse text.
* Support citation form for wordlist / glossary text (update :ref:`<char> <usx-element_char>` @style :ref:`lik <usx-charstyle_w>`).
* Support for explicit :ref:`table <usx-element_table>` :ref:`cell <usx-element_cell>` column spanning (add attribute ``colspan`` to :ref:`cell <usx-element_cell>`).
* Change :ref:`<figure> <usx-element_figure>` :doc:`attribute </attributes>` ``desc`` to ``alt`` to align with companion USFM 3.0 updates to `\\fig ...\\fig* <https://ubsicap.github.io/usfm/master/characters/index.html#fig-fig>`_. 
* *Deprecated* cross reference and footnote DC content :ref:`<char> <usx-element_char>` @style types: :ref:`xdc <usx-note_crossReference_charstyle_xdc>` and :ref:`fdc <usx-note_footnote_charstyle_fdc>`
* *Deprecated* numbered running header :ref:`<para> <usx-element_para>` @style types: :ref:`h# <usx-parastyle_h>`
* *Deprecated* pronunciation info <char> @style pro in favour of ruby glosses :ref:`<char> <usx-element_char>` @style :ref:`rb <usx-charstyle_rb>`.

**Syntax and Features**

* Strategy for applying USX markup to project :doc:`peripheral contents </peripherals>`.
* Standard :ref:`peripheral identifiers <usx-vocab-peripheralIds>`.