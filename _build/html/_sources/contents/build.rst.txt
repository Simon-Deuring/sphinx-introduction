Building the documentation
--------------------------

After you make changes to the source code you must build the project to see the results. To do so, you can open a shell, navigate to the project root and run the folowing command:

.. code-block::

   $ sphinx-build -b html sourcedir builddir

When initializing your project using sphinx-quickstart, a Makefile is added to the directory. This allows to create your HTML pages using a shorter command:

.. code-block::

   $ make html

Running "make" without an argument will show you which targets are available. For example, this shows that you can build to a PDF file using the following command:

.. code-block::

   $ make latexpdf

Please note that this requires a LaTeX engine to be installed on your machine.