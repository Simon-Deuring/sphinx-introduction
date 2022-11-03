Writing your documentation
--------------------------

.. index::
   single: Directives
   single: Arguments
   single: Options
   single: Content

Directives
^^^^^^^^^^

You can use *reStructuredText* directives to define the content of your documentation. Directives can have arguments, options and content. One example is the **toctree** (table of contents tree) directive which is used in the index.rst file to connect multiple files to a single hierarchy of documents. Just add the files you want to include after the **toctree** directive.

.. code-block:: text

   .. toctree::
	  :maxdepth: 2
	  :caption: Contents:
   
	  contents/installation.rst
	  contents/new-project.rst
	  contents/build.rst
	  contents/writing.rst

| In the following a selection of important elements for documentations will be explained. Many more directives can be found under
| https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html.

.. index::
   single: Text highlighting

Text highlighting
^^^^^^^^^^^^^^^^^

Text can easily be highlighted inline using one asterisk before and after a word. This will display the word in italics. Two asterisks lead to an even more highlighted presentation.

* one asterisk for emphasis: ``*text*``
* two asterisks for strong emphasis: ``**text**``
* backquotes for code samples: ````text````

.. index::
   single: Headings

Headings can be highlighted be underlining (and optionally overlining) the section title with a punctuation character, at least as long as the text. The following heading and section types are supported.

* \# with overline, for parts
* \* with overline, for chapters
* \= for sections
* \- for subsections
* \^ for subsubsections
* \" for paragraphs

.. index::
   single: Lists

Lists
^^^^^

If an asterisk is written in front of a line it symbolized an item of an bulleted list. Numbered lists can be created using the hashtag symbol or by writing the item numbers.

.. code-block:: text

   * This code creates a bulleted list.
   * It has two items, the second item
     uses two lines.

   1. This code creates a numbered list.
   2. It also has two items.

   #. This code creates a numbered list.
   #. The items are autonumbered.

You can also nest list of different types.

.. index::
   single: Images

Images
^^^^^^

To visualize certain aspects you can use images. The following code snippet shows the usage of the image directive.

.. code-block:: text

   .. image:: name.png
      (options)

In the options the image width and height can be specified.

.. index::
   single: Code blocks

Code blocks
^^^^^^^^^^^

Finally, you can embed code examples into your documentation by adding a code block directive. In the argument of the directive a programming language can be specified for syntax highlighting.

.. code-block:: java

   .. code-block:: java
   
      public static void main(String[] args) {
	  
      }

If you don't want sytax highlighting you can set the argument to "none" or "text".

.. code-block:: text

   .. code-block:: text
   
      public static void main(String[] args) {
	  
      }