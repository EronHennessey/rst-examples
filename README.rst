
This Sphinx project provides examples of reStructuredText syntax for quick understanding and easy
reference.

Examples are provided in files that describe their contents. For example, `tables.rst <tables.rst>`_
contains examples of writing tables in reST.

Building the examples
=====================

You'll need Sphinx to build the project. If you have ``pip`` installed, you can install it with::

    pip install Sphinx

To build the project, run the following command within the top directory of this repository::

    sphinx-build -b html . _output

