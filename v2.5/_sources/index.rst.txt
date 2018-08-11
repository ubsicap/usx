.. USFM documentation master file, created by
   sphinx-quickstart on Sat Dec 19 21:42:59 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. include:: /_static/inc_styles.txt

.. index:: usx

*****************
USX Documentation
*****************

.. topic:: Welcome

	This is the reference documentation for Unified Scripture XML (USX). USX is an XML format used for encoding the digital text for scripture translations. The largest collection of USX encoded scripture is currently found within the `Digital Bible Library <http://thedigitalbiblelibrary.org>`_.

.. toctree::
   :maxdepth: 1

   Document Structure <structure>
   Elements <elements>
   <para> @style Types <parastyles>
   <char> @style Types <charstyles>
   <note> Types <notes>
   Vocabularies <vocabularies>
   Schemas <schema>

|ico_See| *See also* the documentation :ref:`Index <genindex>` page.

-----

.. note:: **Documentation Syntax Notes**

	Information about individual elements and attributes for XML files within DBL bundles is provided with the following components. Not every component is needed or supplied for each element.
	
	* **Element Description Table:**
	
	   * Required is indicated using a red asterisk (|req|). A plus (+) sign indicates that multiple elements are allowed.
	   * Element attributes are indicated by an "at" symbol **@**
	
	* **Diagram:** A schema diagram is supplied wherever it will assist with clarity; not for every element.
	* **Notes:** Other relevant information not visible in the element description table.
	* **Sample:** An XML sample for the element.
	* **Child Elements:** A list of child elements.
	
	Values for some USX elements are restricted by the USX schema to a pattern or a specific vocabulary. These named patterns (vocabularies) are :doc:`listed <vocabularies>`.
