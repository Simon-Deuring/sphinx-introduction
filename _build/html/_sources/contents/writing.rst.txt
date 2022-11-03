Writing your documentation
--------------------------

You can use *reStructuredText* directives to define the content of your documentation. Directives can have arguments, options and content. One example is the **toctree** (table of contents tree) directive which is used in the index.rst file to connect multiple files to a single hierarchy of documents. Just add the files you want to include after the **toctree** directive.

.. code-block::

   .. toctree::
	  :maxdepth: 2
	  :caption: Contents:
   
	  contents/installation.rst
	  contents/new-project.rst
	  contents/build.rst
	  contents/writing.rst

| In the following a selection of important elements for documentations will be explained. Many more directives can be found under
| https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html.