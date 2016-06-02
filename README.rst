This project provides examples of `reStructuredText <http://docutils.sourceforge.net/rst.html>`_
syntax for quick understanding and easy reference.

Examples are provided in files that describe their contents. For example, `tables.rst <tables.rst>`_
contains examples of writing tables in reST.

Building the examples
=====================

You'll need `Sphinx <http://www.sphinx-doc.org>`_ to build the project. If you have ``pip``
installed, you can install Sphinx with::

    pip install Sphinx

To build the project, run the following command within the top directory of this repository::

    sphinx-build -b html . _output

Then open ``_output/index.html`` in your web browser to view the content.

License
=======

This repository uses the *Creative Commons Zero* license. The text within these files is dedicated
to the **Public Domain**, and you are free to use it in any way you see fit. View the `LICENSE
<LICENSE>`_ for more information.

