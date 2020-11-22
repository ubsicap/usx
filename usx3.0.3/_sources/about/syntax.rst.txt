.. include:: /_static/inc_styles.txt

.. index:: syntax

Syntax Notes
============

.. _syntax_general:
.. index:: syntax; general

General Syntax
--------------

USX follows the `standard syntax <https://www.w3.org/TR/xml/>`_ for XML documents. The :doc:`structure </structure>`, :doc:`elements </elements>`, and :doc:`attributes </attributes>` are derived significantly from the close association USX has with `USFM <https://ubsicap.github.io/usfm>`_ (Unified Standard Format Markers), an older alternative markup scheme for scripture still in widespread use.

.. index:: syntax; documentation
.. _usx-notes_docSyntax:

Documentation Syntax Notes
--------------------------

Information about the individual elements and attributes for USX XML content is provided using the following features in this documentation. Not every feature is needed or supplied for each section of the documentation, or for every element.

* **An element / attribute description table:**

    * The element or attribute name.

        - In the :doc:`<para> </parastyles>`, :doc:`<char> </charstyles>`, and :doc:`<ms> </msstyles>` @style types sections, the tables are primarily providing descriptions for the values of the common attribute ``@style`` which is required for ``<para>``, ``<char>``, and ``<ms>`` elements.

    * Version of USX when the element or attribute was added.
    * Summary of use
    * :doc:`Document structure </structure>` sections within which the element is valid
    * The parent element
    * Required elements or attributes are indicated using a red asterisk (|req|).
    * A plus **+** sign indicates that multiple elements are allowed.
    * Element attributes are indicated by prefixing them with an **@** (at) symbol.
    * Values for some USX elements are restricted by the USX schema to a pattern or a specific vocabulary. Named vocabularies are :doc:`listed </vocabularies>`.

* **Notes:** Other relevant information not visible in the element description table.
* **Text and Formatting Samples:** An XML sample for the element together with a formatted scripture example.

The :doc:`document structure </structure>` presents a USX document as consisting of a sequence of document sections. In the :doc:`Document structure </structure>` section you will also find:

* **Diagram:** A schema diagram is supplied wherever it will promote clarity. These schema diagrams are usually not full expanded since that may present more complexity than needed in most cases -- and since more details for a specific element or attribute can be found elsewhere in the documentation.
* **Child Elements:** A list of the collection of required or optional child elements.
* **Valid @style types:** Document sections are often a collection of one or more para (and nested char elements). For a given section a summary list of valid style types within the section is given.