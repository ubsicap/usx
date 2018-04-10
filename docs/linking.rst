.. include:: /_static/inc_styles.txt

.. index:: usx; linking attributes, attributes; linking
.. _usx-linking_index:

Linking Attributes
==================

|badge_3.0|

USX 3.0 provides a set of attributes for assigning linking properties to :ref:`<char> <usx-element_char>` elements.

.. _usx-linking_syntax:

General Syntax
^^^^^^^^^^^^^^

Linking :doc:`attributes <attributes>` are added using the standard XML syntax. Names given to linking attributes begin with ``link-``, distinguishing them from any other descriptive attributes.

Linking attributes are combined with any other :ref:`descriptive attributes <usx-attributes_descriptive>` added to the same element. The order of attributes is not significant, although it would benefit readability to have descriptive and linking attributes grouped together.

.. note:: 

    When a standard USX scripture reference is required, you must provide a string of pattern: ``[A-Z1-4]{3} ?[a-z0-9\-,:]*``
    
    * Book names must be one of :ref:`bookCode <usx-vocab-bookCode>`
    * Chapter verse separator is always a colon ``:``
    * Verse ranges are indicated using a hyphen
    
    Example: ``MAT 3:1-4``

Attributes
^^^^^^^^^^

:link-href: Identifies the resource being linked to as a URI. |br|

    * Custom USX provided URI prefixes are:

        - ``prj:`` + standard scripture reference. |br| Example: ``prj:RSV52 MAT 3:1-4``
    
    * A link reference within the same project text does not require a URI prefix.
    
    * The resource may be identified by unique id. |br| Example: ``#article-Ruth`` or ``prj:GNTSB #article-Ruth``

:link-title: Plain text describing the remote resource such as might be shown in a tooltip.
:link-id: A unique identifier for this content location (an anchor).

The set of URI prefixes used within a ``link-href`` attribute can be extended beyond the predefined set for USX 3.0. Any user defined URI prefixes must begin with the prefix ``x-``.

**Examples:**

Link to other project text

.. code-block:: xml
    :emphasize-lines: 2

    The traditional translation of verse 1, as given in 
    <char style="jmp" link-href="prj:RSV52 GEN 1:1" link-title="Revised Standard Version">RSV</char>, 
    may be quite appropriate.

Link to illustration / media

.. code-block:: xml
    :emphasize-lines: 2-3

    Storehouses, as used here, refers to large buildings with walls and roof, where grain was 
    kept until needed. (See illustration: <char style="jmp" link-href="figures/storehouse.png" 
    link-title="Ancient storehouse">Storehouse</char>)

Assigning an identifier (anchor). *In this example the markup is a milestone, indicating a location but not marking text.*

.. code-block:: xml
    :emphasize-lines: 5

    <para style="q1">“Someone is shouting in the desert,</para>
    <para style="q2">‘Prepare a road for the Lord;</para>
    <para style="q2">make a straight path for him to travel!’ ”</para>
    <sidebar style="esb" category="people">
      <para style="ms"><char style="jmp" link-id="article-john_the_baptist" />John the Baptist</para>
      <para style="p">John is sometimes called the last “Old Testament prophet” because of the 
        warnings he  brought about God's judgment and because he announced the coming of God's 
        “Chosen One” (Messiah).
      </para>
    </sidebar>

Glossary entry including a link reference to an external URL

.. code-block:: xml

    <char style="w" link-href="http://bibles.org/search/grace/eng-GNTD/all">gracious</char>

Reference to named target within the same project

.. code-block:: xml
    :emphasize-lines: 4

    <para style="p"><verse number="2-6a" style="v" sid="MAT 1:2-6a" />From Abraham to King David, 
      the following ancestors are listed: Abraham, Isaac, Jacob, Judah and his brothers; then Perez 
      and Zerah (their mother was Tamar), Hezron, Ram, Amminadab, Nahshon, Salmon, Boaz (his mother 
      was Rahab), Obed (his mother was <char style="jmp" link-href="#article-Ruth">Ruth</char>), 
      Jesse, and King David.<verse eid="MAT 1:2-6a" />
    </para>

Nested within :ref:`footnote text <usx-note_footnote_charstyle_ft>`

.. code-block:: xml
    :emphasize-lines: 3

    <note caller="-" style="ef"><char style="fr">1.2-6a: </char><char style="fq">Ruth: </char>
      <char style="ft">A Moabite. Only outstanding women were normally included in Jewish 
      genealogical lists. See article on <char style="jmp" link-href="#article-Ruth">Ruth</char>
    </note>

-----

.. _usx-charstyle_jmp-linking:

char @style jmp
^^^^^^^^^^^^^^^

|badge_3.0|

:@style: jmp
:Added: 3.0
:Use: A :doc:`@style type <charstyles>` value for use with :ref:`<char> <usx-element_char>`. Available for associating linking attributes to a span of text when no other :ref:`<char> <usx-element_char>` element is already applied to the text at this location.
:Valid In: Any valid :ref:`usx-element_char`

*Linking examples provided above*