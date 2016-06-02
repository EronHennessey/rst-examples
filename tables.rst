#######################
reStructuredText Tables
#######################

Here are some examples of different types of tables in reStructuredText.

Ascii tables
============

Ascii table type 1
------------------

The most ascii-art intensive table is the only table type that allows you to span columns. Header
rows are separated from the rest of the table by a line of ``=`` characters. Rows are separated by
lines of ``-`` characters, and ``+`` symbols are used for the corners of cells.

.. code-block:: rst

    +---------------+---------------+
    | header item 1 | header item 2 |
    +===============+===============+
    | cell 1 (span)                 |
    +---------------+---------------+
    | cell 2        | cell 3        |
    +---------------+---------------+

Renders as:

+---------------+---------------+
| header item 1 | header item 2 |
+===============+===============+
| cell 1 (span)                 |
+---------------+---------------+
| cell 2        | cell 3        |
+---------------+---------------+


Ascii table type 2
------------------

This style of ascii table uses columns separated by spaces. Boundaries are drawn using ``=``
characters, including separating headers from the rest of the table; table rows are separated by
newlines.

.. code-block:: rst

    =============  =============
    header item 1  header item 2
    =============  =============
    cell 1
    cell 2         cell 3
    =============  =============

Renders as:

=============  =============
header item 1  header item 2
=============  =============
cell 1
cell 2         cell 3
=============  =============


Ascii table 3
-------------

Not really a different table type, but you can *provide a title* for an ascii table by using the
:rst-directive:`table` directive:

.. code-block:: rst

   .. table:: *This table has a title!*

       +---------------+---------------+
       | header item 1 | header item 2 |
       +===============+===============+
       | cell 1 (span)                 |
       +---------------+---------------+
       | cell 2        | cell 3        |
       +---------------+---------------+

Renders as:

.. table:: *This table has a title!*

    +---------------+---------------+
    | header item 1 | header item 2 |
    +===============+===============+
    | cell 1 (span)                 |
    +---------------+---------------+
    | cell 2        | cell 3        |
    +---------------+---------------+


CSV tables
==========

The :rst-directive:`csv-table` directive allows you to provide rows of text, with cells separated by
commas.

.. code-block:: rst

   .. csv-table::
      :header-rows: 1
      :widths: 2, 3

      "header item 1", "header item 2"
      "cell 1"
      "cell 2", "cell 3"

Renders as:

.. csv-table::
   :header-rows: 1
   :widths: 2, 3

   "header item 1", "header item 2"
   "cell 1"
   "cell 2", "cell 3"


List tables
===========

:rst-directive:`List tables <list-table>` are written by using list items to separate rows, each
with a sub-list to define cells within the row. In addition to being very easy to read in text
format, they're ideal for arbitrary cell content, including images, code blocks, admonitions and
other directives.

.. code-block:: rst

   .. list-table::
      :header-rows: 1
      :widths: 2, 3

      - * header item 1
        * header item 2

      - * cell 1
        * .. image:: _static/Purr.png

      - * cell 2
        * cell 3

Renders as:

.. list-table::
   :header-rows: 1
   :widths: 2, 3

   - * header item 1
     * header item 2

   - * cell 1
     * .. image:: _static/Purr.png

   - * cell 2
     * cell 3

