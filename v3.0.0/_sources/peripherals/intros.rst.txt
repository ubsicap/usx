.. include:: /_static/inc_styles.txt

.. index:: book@code; INT, peripherals; Introductions, introductions
.. _usx-book_INT:

Introductions
=============

The INT :ref:`book <usx-element_book>` and its :ref:`divisions <usx-peripherals_div>` can be used for storing introductory material related to the various book groupings within a scripture publication. This material has also been referred to as “mid-matter”.

**General**

Use the following :doc:`elements </elements>` (or other appropriate USX elements and :doc:`<para> </parastyles>` or :doc:`<char> </charstyles>` @style types, as required) to create introduction content for specific :ref:`divisions <usx-peripherals_div>`.

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`m <usx-parastyle_m>` - Flush left (margin) paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`pi# <usx-parastyle_pi>` - Indented paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`li# <usx-parastyle_li>` - List item.
* :ref:`<para> <usx-element_para>` @style :ref:`q# <usx-parastyle_q>` - Poetic line.
* :ref:`<table> <usx-element_table>` - For any tabular data.
* :ref:`<char> <usx-element_char>` @style :ref:`bk <usx-charstyle_bk>`, :ref:`qt <usx-charstyle_qt>`, :ref:`tl <usx-charstyle_tl>` or other <char> @style types.
* :ref:`<figure> <usx-element_figure>` - Figure.

**Text Samples**

.. code-block:: xml
    :name: usx-peripherals_intot_example
    :emphasize-lines: 4,12

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="INT" style="id" />
        <periph alt="Old testament Introduction" id="intot">
            <para style="mt1">Introduction to the Old Testament</para>
            <para style="p">The Old Testament is a record of Israel's experience of what God is like 
                and what the people who worship God should be like. It proclaims the LORD God as the 
                creator of the world and it tells how God blesses people and establishes relations with 
                people through special agreements called covenants.
            </para>
            ...
        </periph>
    </usx>

.. code-block:: xml
    :name: usx-peripherals_intpent_example
    :emphasize-lines: 4,11

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="INT" style="id" />
        <periph alt="Pentateuch Introduction" id="intpent">
            <para style="mt1">The Pentateuch</para>
            <para style="p">“Pentateuch” is a term that means “five scrolls (books)” and is used to 
                describe the five books that are positioned at the beginning of both Jewish and 
                Christian Bibles.
            </para>
            ...
        </periph>
    </usx>

.. code-block:: xml
    :name: usx-peripherals_intnt_example
    :emphasize-lines: 4,10

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="INT" style="id" />
        <periph alt="New Testament Introduction" id="intnt">
            <para style="mt1">Introduction to the New Testament</para>
            <para style="p">The books of the New Testament were written by the followers of
                Jesus Christ...
            </para>
            ...
        </periph>
    </usx>

.. code-block:: xml
    :name: usx-peripherals_intgospels_example
    :emphasize-lines: 4,8

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="INT" style="id" />
        <periph alt="Gospels Introduction" id="intgospels">
            <para style="mt1">Gospels and Acts</para>
            <para style="p">...</para>
            ...
        </periph>
    </usx>
