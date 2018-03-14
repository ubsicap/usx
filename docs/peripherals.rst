.. include:: /_static/inc_styles.txt

.. index:: element; <periph>, peripherals
.. _usx-peripherals_index:

Peripherals
===========

|badge_3.0|

The following strategy should be used for applying USX markup to project peripheral contents.

Content should be created in separate files according to the general groupings presented in the table below. As with scripture text books, a :ref:`book <usx-element_book>` element with appropriate ``@code`` attribute is used for identifying the overall content of the peripheral file. Within each peripheral file, divisions (sub-sections) of content are denoted using the element :ref:`<periph> <usx-element_periph>` followed by an additional division title. Content is added to books and divisions by re-purposing the most appropriate existing USFM marker for the selected content.

Some back matter content is large enough that it is most practical to store it within its own book file (Concordance, Glossary, Topical Index, Names Index). Content self contained within a separate book file does not require an additional identifier (only :ref:`book <usx-element_book>` ``@code``).

.. _usx-peripherals_div:
.. _usx-vocab-peripheralIds:
.. index:: pair: peripherals; books
	pair: peripherals; divisions

Peripheral Books and Divisions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+------------------------------------------+----------------------------------------------+----------------------------------------+
| :doc:`Front Matter <peripherals/front>`  | :doc:`Introductions <peripherals/intros>`    | :doc:`Back Matter <peripherals/back>`  |
| |br| ``<book code="FRT" style="id">``    | |br| ``<book code="INT" style="id">``        | |br| ``<book code="BAK" style="id">``  |
+==========================================+==============================================+========================================+
| **Divisions**                            | **Divisions**                                | **Divisions**                          |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | ``<periph``                            |
| |br| ``alt="Title Page"``                | |br| ``alt="Bible Introduction"``            | |br| ``alt="Chronology"``              |
| |br| ``id="title">``                     | |br| ``id="intbible">``                      | |br| ``id="chron">``                   |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | ``<periph``                            |
| |br| ``alt="Half Title Page"``           | |br| ``alt="Old Testament Introduction"``    | |br| ``alt="Weights and Measures"``    |
| |br| ``id="halftitle">``                 | |br| ``id="intot">``                         | |br| ``id="measures">``                |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | ``<periph``                            |
| |br| ``alt="Promotional Page"``          | |br| ``alt="Pentateuch Introduction"``       | |br| ``alt="Map Index"``               |
| |br| ``id="promo">``                     | |br| ``id="intpent">``                       | |br| ``id="maps">``                    |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | ``<periph``                            |
| |br| ``alt="Imprimatur"``                | |br| ``alt="History Introduction"``          | |br| ``alt="LXX Quotes in NT"``        |
| |br| ``id="imprimatur">``                | |br| ``id="inthistory">``                    | |br| ``id="lxxquotes">``               |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | **Additional Back Matter**             |
| |br| ``alt="Publication Data"``          | |br| ``alt="Poetry Introduction"``           |                                        |
| |br| ``id="pubdata">``                   | |br| ``id="intpoetry">``                     |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | :ref:`Concordance <usx-book_CNC>`      |
| |br| ``alt="Foreword"``                  | |br| ``alt="Prophecy Introduction"``         | |br| ``<book code="CNC" style="id">``  |
| |br| ``id="foreword">``                  | |br| ``id="intprophesy">``                   |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | :ref:`Glossary <usx-book_GLO>`         |
| |br| ``alt="Preface"``                   | |br| ``alt="Deuterocanon Introduction"``     | |br| ``<book code="GLO" style="id">``  |
| |br| ``id="preface">``                   | |br| ``id="intdc">``                         |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | :ref:`Topical Index <usx-book_GLO>`    |
| |br| ``alt="Table of Contents"``         | |br| ``alt="New Testament Introduction"``    | |br| ``<book code="TDX" style="id">``  |
| |br| ``id="contents">``                  | |br| ``id="intnt">``                         |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | :ref:`Names Index <usx-book_TDX>`      |
| |br| ``alt="Alphabetical Contents"``     | |br| ``alt="Gospels Introduction"``          | |br| ``<book code="NDX" style="id">``  |
| |br| ``id="alphacontents">``             | |br| ``id="intgospels">``                    |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
| ``<periph``                              | ``<periph``                                  | :doc:`Other <peripherals/other>`       |
| |br| ``alt="Table of Abbreviations"``    | |br| ``alt="Epistles Introduction"``         | |br| ``<book code="OTH" style="id">``  |
| |br| ``id="abbreviations">``             | |br| ``id="intepistles">``                   |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
|                                          | ``<periph``                                  | **Divisions**                          |
|                                          | |br| ``alt="Letters Introduction"``          |                                        |
|                                          | |br| ``id="intletters">``                    |                                        |
+------------------------------------------+----------------------------------------------+----------------------------------------+
|                                          |                                              | ``<periph``                            |
|                                          |                                              | |br| ``alt="Cover"``                   |
|                                          |                                              | |br| ``id="cover">``                   |
+------------------------------------------+----------------------------------------------+----------------------------------------+
|                                          |                                              | ``<periph``                            |
|                                          |                                              | |br| ``alt="Spine"``                   |
|                                          |                                              | |br| ``id="spine">``                   |
+------------------------------------------+----------------------------------------------+----------------------------------------+

.. _usx-peripherals_Ids:
.. _usx-attributes_peripheralIds:
.. index:: peripherals; identifiers, attribute; periph@id

Peripheral Identifiers
^^^^^^^^^^^^^^^^^^^^^^

For books containing a peripheral :ref:`division <usx-peripherals_div>`, the :ref:`<periph> <usx-element_periph>` container element should identify the content using a standard peripheral identifier ``id`` attribute. The defined ``id`` values are shown in the peripheral :ref:`divisions <usx-peripherals_div>` table above. The set of standardized identifiers allow software processes to easily select content for recognized peripheral divisions. The :ref:`<periph> <usx-element_periph>` element's ``alt`` attribute provides an alternate title or identifier (possibly vernacular) for the peripheral content.

**Text samples with peripheral division identifier attributes:**

.. code-block:: xml
	:name: usx-peripherals_title_example
	:emphasize-lines: 4,8
    
	<?xml version="1.0" encoding="utf-8"?>
	<usx version="3.0">
		<book code="FRT" style="id">Good News Translation Front Matter</book>
		<periph alt="Title Page" id="title">
			<para style="mt1">Holy Bible</para>
			<para style="mt3">with</para>
			<para style="mt2">Deuterocanonicals/Apocrypha</para>
		</periph>
	</usx>

.. code-block:: xml
	:name: usx-peripherals_foreword_example
	:emphasize-lines: 4,13
	
	<?xml version="1.0" encoding="utf-8"?>
	<usx version="3.0">
		<book code="FRT" style="id">Good News Translation Front Matter</book>
		<periph alt="Foreword" id="foreword">
			<para style="h">Foreword</para>
			<para style="mt1">Foreword</para>
			<para style="p">The <char style="bk">Good News
			Translation</char> of the Bible is a translation which 
			seeks to state clearly and accurately the meaning of the 
			original texts in words and forms that are widely accepted 
			by people who use English as a means of 
			communication.</para>
		</periph>
	</usx>

.. code-block:: xml
	:name: usx-peripherals_contents_example
	:emphasize-lines: 4,24
	
	<?xml version="1.0" encoding="utf-8"?>
	<usx version="3.0">
		<book code="FRT" style="id">Good News Translation Front Matter</book>
		<periph alt="Table of Contents" id="contents">
			<para style="h">Contents</para>
			<para style="mt1">Contents</para>
			<para style="s">Old Testament</para>
			<table>
				<row style="tr">
					<cell style="th1" align="start">Name</cell>
					<cell style="th2" align="start">Page</cell>
					<cell style="th3" align="start">Name</cell>
					<cell style="th3" align="start">Page</cell>
				</row>
				<row style="tr">
					<cell style="th1" align="start">Genesis</cell>
					<cell style="th2" align="start">#</cell>
					<cell style="th3" align="start">Ecclesiastes</cell>
					<cell style="th3" align="start">#</cell>
				</row>
				...
			</table>
			...
		</periph>
	</usx> 

.. _usx-peripherals_div-user:
.. index:: peripherals; user defined divisions

User Defined Peripheral Divisions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A project may add peripheral content for a division not defined in the current USX set. The new division should be enclosed in :ref:`<periph> <usx-element_periph>` container element and with a user defined ``id`` attribute beginning with the prefix ``x-``.

USX compliant publishing applications should consider the pre-defined :ref:`divisions <usx-peripherals_div>` and identifiers as a reference for content to support.

Markup for Peripheral Divisions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In the following topics there is a recommendation and a brief description of the USX :doc:`<para> <parastyles>` and :doc:`<char> <charstyles>` @style types which will be most appropriate for use in each peripheral content :ref:`division <usx-peripherals_div>`. The recommended markup is sufficient for most projects and should be used as a first option. However, in general, any suitable :doc:`<para> <parastyles>` and :doc:`<char> <charstyles>` @style types may be used if the required content cannot be adequately encoded using the recommended set.

.. toctree::
   :maxdepth: 1

   Front Matter <peripherals/front>
   Introductions <peripherals/intros>
   Back Matter <peripherals/back>
   Other <peripherals/other>