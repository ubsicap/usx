.. include:: /_static/inc_styles.txt

.. index:: book@code; BAK, peripherals; Back Matter, back matter
.. _usx-book_BAK:

Back Matter
===========

The BAK :ref:`book <usx-element_book>` and its :ref:`divisions <usx-peripherals_div>` can be used for storing material which is typically presented at the end of a scripture publication. In practice some back matter content is large enough to require storing it in its own book file (:ref:`Concordance <usx-book_CNC>`, :ref:`Glossary <usx-book_GLO>`, :ref:`Topical Index <usx-book_TDX>`, :ref:`Names Index <usx-book_NDX>`).

**General**

Use the following :doc:`elements </elements>` (or other appropriate USX elements and :doc:`<para> </parastyles>` or :doc:`<char> </charstyles>` @style types, as required) to create back matter information or introductory content for specific :ref:`divisions <usx-peripherals_div>`.

.. index:: periph@id; chron, peripherals; Chronology, chronology

Chronology
^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<table> <usx-element_table>` - For any tabular data.

.. index:: periph@id; measures, peripherals; Weights and Measures, weights and measures

Weights and Measures
^^^^^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<table> <usx-element_table>` - For any tabular data.

.. index:: periph@id; maps, peripherals; Map Index, map index

Map Index
^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<table> <usx-element_table>` - For any tabular data.
* :ref:`<char> <usx-note_crossReference_char>` @style type :ref:`xt <usx-note_crossReference_charstyle_xt>` - Index target references.

**Text Sample**

In the following example, the variable # represents the location of a page number, to be inserted during the typesetting process.

.. code-block:: xml
    :name: usx-peripherals_maps_example
    :emphasize-lines: 4,55
    
    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="BAK" style="id">English: Good News Translation 2nd Ed. 1992</book>
        <periph alt="Map Index" id="maps">
            <para style="mt1">Map Index</para>
            ...
            <para style="ip">This atlas contains the following maps. Since a number of these maps 
            are especially helpful when reading specific books of the Bible, some have also been 
            placed within the text of the Bible. The page number indicated below will help you find 
            these maps both within the text and within this atlas.</para>
            <table>
                <row style="tr">
                    <cell style="th1" align="start">Map </cell>
                    <cell style="thr2" align="end">Page </cell>
                </row>
                <row style="tr">
                    <cell style="tc1" align="start">Ancient World </cell>
                    <cell style="tc2" align="start"># </cell>
                </row>
                <row style="tr">
                    <cell style="tc1" align="start">Egypt and Sinai </cell>
                    <cell style="tc2" align="start"># </cell>
                </row>
                <row style="tr">
                    <cell style="tc1" align="start">Division of Canaan </cell>
                    <cell style="tc2" align="start"># </cell>
                </row>
                <row style="tr">
                    <cell style="tc1" align="start">United Israelite Kingdom </cell>
                    <cell style="tc2" align="start"># </cell>
                </row>
                ...
            </table>
            <para style="s1">Index to Places</para>
            <para style="s2">A</para>
            <table>
                <row style="tr">
                    <cell style="tc1" align="start">A </cell>
                    <cell style="tc2" align="start">Baal Zephon</cell>
                    <cell style="tc3" align="start">[B]</cell>
                </row>
                <row style="tr">
                    <cell style="tc1" align="start">A </cell>
                    <cell style="tc2" align="start">Babylon</cell>
                    <cell style="tc3" align="start">[E]</cell>
                </row>
                <row style="tr">
                    <cell style="tc1" align="start">B </cell>
                    <cell style="tc2" align="start">Babylonia</cell>
                    <cell style="tc3" align="start">[E]</cell>
                </row>
                ...
            </table>
            ...
        </periph>
    </usx>

.. index:: periph@id; lxxquotes, peripherals; NT Quotes from LXX, NT quotes from LXX

NT Quotes from LXX
^^^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_p>` - Paragraph.
* :ref:`<char> <usx-element_char>` @style :ref:`k <usx-charstyle_k>` - Keyword.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_lxxquotes_example
    :emphasize-lines: 4,16
    
    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="BAK" style="id">English: Good News Translation 2nd Ed. 1992</book>
        <periph alt="Map Index" id="maps">
            <para style="ip">The writers of the New Testament generally quoted or paraphrased the 
                ancient Greek translation of the Old Testament, commonly known as the Septuagint 
                Version (LXX), made some two hundred years before the time of Christ.
            ...
            <para style="p"><char style="k">Matthew 1.23</char> (Isaiah 7.14) A virgin will become 
                pregnant and have a son. 
            <para style="p"><char style="k">Matthew 3.3</char> (Isaiah 40.3) Someone is shouting in 
                the desert, “Prepare a road for the Lord; make a straight path for our God to travel!” 
            <para style="p"><char style="k">Matthew 12.21</char> (Isaiah 42.4) And on him all people 
                will put their hope.
            ...
        </periph>
    </usx>

-----

The following back matter content should each be created within their own :ref:`book <usx-element_book>` file.

.. _usx-book_CNC:
.. index:: book@code; CNC, peripherals; concordance, concordance

Concordance
^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading (e.g. headings of alphabetical divisions - "A", "B", "C" etc.)
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Main entry + example "cut string" *(required)*.
* :ref:`<char> <usx-element_char>` @style :ref:`k <usx-charstyle_k>` - Main entry keyword *(required)*.
* :ref:`<para> <usx-element_para>` @style :ref:`d <usx-parastyle_d>` - Keyword description.
* :ref:`<char> <usx-note_crossReference_char>` @style type :ref:`xt <usx-note_crossReference_charstyle_xt>` - Entry target reference(s) *(required)*. Use of :ref:`<ref> <usx-element_ref>` elements in the text sample is optional.
* :ref:`<char> <usx-element_char>` @style :ref:`bd <usx-charstyle_bd>` - Highlight of the main entry within the cut string (bold).
* :ref:`<para> <usx-element_para>` @style :ref:`pi# <usx-parastyle_pi>` - Sub-entries, or secondary paragraph(s) (if indentation is preferred).
* :ref:`<char> <usx-element_char>` @style :ref:`add <usx-charstyle_add>` - Grammar abbreviation (optional).
* :ref:`<table> <usx-element_table>` - For any tabular data.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_cnc_example
    :emphasize-lines: 3

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="CNC" style="id" />
        <para style="mt">Concordance</para>
        <para style="ip">The entries in this concordance have been carefully selected by a team of 
            editors. They have aimed to include all of the verses most likely to be looked up.</para>
        <para style="ip">A concordance of this size cannot include every occurrence of each 
            individual word.</para>
        ...
        <para style="s">A</para>
        <para style="p"><char style="k">Abandon</char></para>
        <para style="p"><char style="xt"><ref loc="LEV 19:4">Lev 19.4</ref></char>Do not 
            <char style="bd">abandon</char> me and worship idols.</para>
        <para style="p"><char style="xt"><ref loc="DEU 31:6">Deu 31.6</ref></char>He will not fail you 
            or <char style="bd">abandon</char> you.”</para>
        <para style="p"><char style="xt"><ref loc="DEU 32:15">Deu 32.15</ref></char>They 
            <char style="bd">abandoned</char> God their Creator</para>
        ...
        <para style="p"><char style="k">Able</char></para>
        <para style="p"><char style="xt"><ref loc="EXO 31:3">Exo 31.3</ref></char> understanding, skill, 
            and <char style="bd">ability</char></para>
        <para style="p"><char style="xt"><ref loc="DAN 3:17">Dan 3.17</ref></char> If the God whom we 
            serve is <char style="bd">able</char></para>
        <para style="p"><char style="xt"><ref loc="MAT 26:61">Mat 26.61</char> and said, “This man said, 
            ‘I am <char style="bd">able</char></para>
        ...
        <para style="s">B</para>
        ...
    </usx>

.. _usx-book_GLO:
.. index:: book@code; GLO, peripherals; Glossary, glossary

Glossary
^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading (e.g. headings of alphabetical divisions - "A", "B", "C" etc.)
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Main entry *(required)*. May also be used for any additional paragraphs in the definition entry (optional).
* :ref:`<char> <usx-element_char>` @style :ref:`k <usx-charstyle_k>` - Main entry keyword *(required)*.
* :ref:`<para> <usx-element_para>` @style :ref:`pi# <usx-parastyle_pi>` - Sub-entries, or secondary paragraph(s) (if indentation is preferred).
* :ref:`<para> <usx-element_para>` @style :ref:`li# <usx-parastyle_li>` - List item.
* :ref:`<char> <usx-element_char>` @style :ref:`tl <usx-charstyle_tl>` - National idiom word(s).

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_glo_example
    :emphasize-lines: 3

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="GLO" style="id" />
        <para style="mt">Glossary</para>
        <para style="ip">This dictionary is divided into 21 sections. The indexes below list all of the 
            sections, and all of the entries in alphabetical order, so that you can find what you 
            are looking for more easily.
        <para style="s">A</para>
        <para style="p"><char style="k">Angel</char>A supernatural being who tells God's 
            messages to people or protects those who belong to God.
        ...
        <para style="s">C</para>
        <para style="p"><char style="k">Council</char>(1) A group of leaders who meet and make decisions 
            for their people.
        <para style="pi">(2) The Old Testament refers to God's council as a group of angels who meet and 
            talk with God in heaven.
	    ...
    </usx>

.. _usx-book_TDX:
.. index:: book@code; TDX, peripherals; Topical Index, topical index

Topical Index
^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading (e.g. headings of alphabetical divisions - "A", "B", "C" etc.)
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Main entry *(required)*. May also be used for any additional paragraphs in the definition entry (optional).
* :ref:`<char> <usx-element_char>` @style :ref:`k <usx-charstyle_k>` - Main entry keyword *(required)*.
* :ref:`<char> <usx-note_crossReference_char>` @style type :ref:`xt <usx-note_crossReference_charstyle_xt>` - Entry target reference(s) *(required)*. More than one <char style="xt"> ...</char> element can be provided to create logical groupings of references (per chapter; per book etc.). Use of :ref:`<ref> <usx-element_ref>` elements in the text sample is optional.
* :ref:`<para> <usx-element_para>` @style :ref:`pi# <usx-parastyle_pi>` - Sub-entries, or secondary paragraph(s) (if indentation is preferred).
* :ref:`<para> <usx-element_para>` @style :ref:`li# <usx-parastyle_li>` - Use for simple lists, where more complex tabular layout is not required.
* :ref:`<table> <usx-element_table>` - For any tabular data.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_tdx_example
    :emphasize-lines: 3

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="TDX" style="id" />
        <para style="mt">Topical Index</para>
        <para style="ip">Introductory paragraph(s)</para>
        ...
        <para style="s">A</para>
        <para style="p"><char style="k">Aaron</char>
            <char style="xt"><ref loc="ACT 7:40">Act 7.40</ref></char>
            <char style="xt"><ref loc="HEB 5:4">Heb 5.4</ref>; <ref loc="HEB 7:11">7.11</ref>; 
            <ref loc="HEB 9:4>">9.4</ref></char>
        </para>
        ...
        <para style="p"><char style="k">Angels</char></para>
        <para style="pi">(a) messengers and agents of God
            <char style="xt"><ref loc="MAT 1:20-24">Mat 1.20-24</ref>; <ref loc="MAT 4:11">4.11</ref>; 
                <ref loc="MAT 13:39">13.39</ref>,<ref loc="MAT 13:41">41</ref>,
                <ref loc="MAT 13:49">49</ref>; <ref loc="MAT 16:27">16.27</ref>; 
                <ref loc="MAT 34:31">34.31</ref>; <ref loc="MAT 25:31">25.31</ref>; 
                <ref loc="MAT 28:2-7">28.2-7</ref></char>
            <char style="xt"><ref loc="LUK 1:11-19">Luk 1.11-19</ref>; 
                <ref loc="LUK 11:26-38">26-38</ref>; <ref loc="LUK 2:9-21">2.9-21</ref></char>
            <char style="xt"><ref loc="JHN 1:51">Jhn 1.51</ref></char>
        </para>
        ...
        <para style="pi">(b) in heaven
            <char style="xt"><ref loc="MAT 22:30">Mat 22.30</ref></char>
            <char style="xt"><ref loc="LUK 12:8-9">Luk 12.8-9</ref>; <ref loc="LUK 15:10">15.10</ref>; 
                <ref loc="LUK 20:36">20.36</ref></char>
        </para>
        ...
    </usx>


.. _usx-book_NDX:
.. index:: book@code; NDX, peripherals; Names Index, names index

Names Index
^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`is# <usx-parastyle_is>` - Introduction heading.
* :ref:`<para> <usx-element_para>` @style :ref:`ip <usx-parastyle_ip>` - Introduction paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading (e.g. headings of alphabetical divisions - "A", "B", "C" etc.)
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Main entry *(required)*. May also be used for any additional paragraphs in the definition entry (optional).
* :ref:`<char> <usx-element_char>` @style :ref:`k <usx-charstyle_k>` - Main entry keyword *(required)*.
* :ref:`<char> <usx-note_crossReference_char>` @style type :ref:`xt <usx-note_crossReference_charstyle_xt>` - Entry target reference(s) *(required)*. More than one <char style="xt"> ...</char> element can be provided to create logical groupings of references (per chapter; per book etc.). Use of :ref:`<ref> <usx-element_ref>` elements in the text sample is optional.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_ndx_example
    :emphasize-lines: 3

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="NDX" style="id" />
        <para style="mt">Names Index</para>
        <para style="ip">Introductory paragraph(s) ...</para>
        ...
        <para style="s">A</para>
        <para style="p"><char style="k">Aaron</char>
            <char style="xt"><ref loc="EXO 4:14-30">Exo 4.14-30</ref> (x5)</char>
            <char style="xt"><ref loc="EXO 5:1-21">Exo 5.1-21</ref> (x5)</char>
        </para>
        ...
        <para style="p"><char style="k">Abraham</char>
        <para style="p">See Also 
            <char style="jmp" link-href="#ndx-Abram" link-title="Entry for Abram">Abram</char>
            <char style="xt"><ref loc="GEN 17:5-27">Gen 17.5-27</ref> (x8)</char>
            <char style="xt"><ref loc="GEN 18:1-33">Gen 18.1-33</ref> (x15)</char>
        </para>
        ...
        <para style="s">B</para>
        <para style="p"><char style="k">Baal</char>
            <char style="xt"><ref loc="NUM 22:41">Num 22.41</ref></char>
            <char style="xt"><ref loc="NUM 25:3-5">Num 25.3-5</ref> (x2)</char>
        </para>
    </usx>