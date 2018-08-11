.. include:: /_static/inc_styles.txt

.. index:: book@code; FRT, peripherals; Front Matter, front matter
.. _usx-book_FRT:

Front Matter
============

The FRT :ref:`book <usx-element_book>` and its :ref:`divisions <usx-peripherals_div>` can be used for storing material which is typically presented at the start of a scripture publication, before the first book of scripture.

**General**

Use the following :doc:`elements </elements>` (or other appropriate USX elements and :doc:`<para> </parastyles>` or :doc:`<char> </charstyles>` @style types, as required) to create front matter information or introductory content for specific :ref:`divisions <usx-peripherals_div>`.

.. index:: periph@id; title, peripherals; Title Page, title page

Title Page
^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`pc <usx-parastyle_pc>` - Centered paragraph.
* :ref:`<figure> <usx-element_figure>` - Figure.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_title_example
    :emphasize-lines: 4,16

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="FRT" style="id" />
        <periph alt="Title Page" id="title">
            <para style="mt1">Holy Bible</para>
            <para style="mt3">with</para>
            <para style="mt2">Deuterocanonicals/Apocrypha</para>
            <para style="pc">Good News Translation</para>
            <para style="pc">
                <figure style="fig" desc="GNT Logo" file="gntLogo.jpg" size="span" loc="" copy="" ref="" />
            </para>
            <para style="pc">
                <figure style="fig" desc="ABS Logo" file="absLogo.jpg" size="span" loc="" copy="" ref="" />
            </para>
            <para style="pc">American Bible Society</para>
        </periph>
    </usx>

.. index:: periph@id; halftitle, peripherals; Half Title Page, half title page

Half Title Page
^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`pc <usx-parastyle_pc>` - Centered paragraph.
* :ref:`<figure> <usx-element_figure>` - Figure.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_halftitle_example
    :emphasize-lines: 4,10

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="FRT" style="id" />
        <periph alt="Half Title Page" id="halftitle">
            <para style="mt1">Holy Bible</para>
            <para style="pc">Good News Translation</para>
            <para style="pc">
                <figure style="fig" desc="GNT Logo" file="gntLogo.jpg" size="span" loc="" copy="" ref="" />
            </para>
        </periph>
    </usx>

.. index:: periph@id; promo, peripherals; Promotional Page, promotional page

Promotional Page
^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`m <usx-parastyle_m>` - Flush left (margin) paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`pi# <usx-parastyle_pi>` - Indented paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`li# <usx-parastyle_li>` - List item.
* :ref:`<para> <usx-element_para>` @style :ref:`q# <usx-parastyle_q>` - Poetic line.

.. index:: periph@id; imprimatur, peripherals; Imprimatur, imprimatur

Imprimatur
^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`pc <usx-parastyle_pc>` - Centered paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Paragraph.
* :ref:`<table> <usx-element_table>` - For any tabular data.
* :ref:`<figure> <usx-element_figure>` - Figure.

.. index:: periph@id; pubdata, peripherals; Publication Data, publication data

Publication Data
^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`pc <usx-parastyle_pc>` - Centered paragraph.
* :ref:`<para> <usx-element_para>` @style :ref:`p <usx-parastyle_p>` - Paragraph.
* :ref:`<table> <usx-element_table>` - For any tabular data.

.. index:: periph@id; foreword, peripherals; Foreword, foreword

Foreword
^^^^^^^^

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

.. index:: periph@id; preface, peripherals; Preface, preface

Preface
^^^^^^^

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

.. index:: periph@id; contents, peripherals; Contents, contents

Table of Contents
^^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<table> <usx-element_table>` - For any tabular data.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_contents_example
    :emphasize-lines: 4,50

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="FRT" style="id" />
        <periph alt="Table of Contents" id="contents">
            <para style="mt1">Contents</para>
            <para style="s1">Old Testament</para>
            <table>
                <row style="tr">
                    <cell style="th1" align="start">Name</cell>
                    <cell style="th2" align="end">Page</cell>
                    <cell style="th3" align="start">Name</cell>
                    <cell style="th4" align="end">Page</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Genesis</cell>
                    <cell style="th2" align="end">#</cell>
                    <cell style="th3" align="start">Ecclesiastes</cell>
                    <cell style="th4" align="end">#</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Exodus</cell>
                    <cell style="th2" align="end">#</cell>
                    <cell style="th3" align="start">Song of Songs</cell>
                    <cell style="th4" align="end">#</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Leviticus</cell>
                    <cell style="th2" align="end">#</cell>
                    <cell style="th3" align="start">Isaiah</cell>
                    <cell style="th4" align="end">#</cell>
                </row>
                ...
            </table>
            <para style="s1">New Testament</para>
            <table>
                <row style="tr">
                    <cell style="th1" align="start">Name</cell>
                    <cell style="th2" align="end">Page</cell>
                    <cell style="th3" align="start">Name</cell>
                    <cell style="th4" align="end">Page</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Matthew</cell>
                    <cell style="th2" align="end">#</cell>
                    <cell style="th3" align="start">1 Timothy</cell>
                    <cell style="th4" align="end">#</cell>
                </row>
                ...
            </table>
        </periph>
    </usx>

.. index:: periph@id; alphacontents, peripherals; Alphabetical Content, alphabetical contents

Alphabetical Contents
^^^^^^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<table> <usx-element_table>` - For any tabular data.

.. index:: periph@id; abbreviations, peripherals; Table of Abbreviations, table of abbreviations

Table of Abbreviations
^^^^^^^^^^^^^^^^^^^^^^

* :ref:`<para> <usx-element_para>` @style :ref:`mt# <usx-parastyle_mt>` - Main title.
* :ref:`<para> <usx-element_para>` @style :ref:`s# <usx-parastyle_s>` - Section heading.
* :ref:`<table> <usx-element_table>` - For any tabular data.

**Text Sample**

.. code-block:: xml
    :name: usx-peripherals_abbreviations_example
    :emphasize-lines: 4,43

    <?xml version="1.0" encoding="utf-8"?>
    <usx version="3.0">
        <book code="FRT" style="id" />
        <periph alt="Table of Abbreviations" id="abbreviations">
            <para style="mt1">Alphabetical List of Biblical Books and Abbreviations</para>
            <table>
                <row style="tr">
                    <cell style="th1" align="start">Name</cell>
                    <cell style="th2" align="start">Abbrev.</cell>
                    <cell style="th3" align="end">Page</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Acts</cell>
                    <cell style="th2" align="start">Ac</cell>
                    <cell style="th3" align="end">#</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Amos</cell>
                    <cell style="th2" align="start">Am</cell>
                    <cell style="th3" align="end">#</cell>
                </row>
                ...
            </table>
            <para style="s1">Other Abbreviations</para>
            <table>
                <row style="tr">
                    <cell style="th1" align="start">Term</cell>
                    <cell style="th2" align="start">Abbrev.</cell>
                    <cell style="th3" align="end">Page</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Circa (around)</cell>
                    <cell style="th2" align="start">c</cell>
                    <cell style="th3" align="end">#</cell>
                </row>
                <row style="tr">
                    <cell style="th1" align="start">Old Testament</cell>
                    <cell style="th2" align="start">OT</cell>
                    <cell style="th3" align="end">#</cell>
                </row>
                ...
            </table>
        </periph>
    </usx>