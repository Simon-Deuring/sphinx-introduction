.. index::
   single: Installation

Installation
------------

.. index::
   single: Windows

Windows
^^^^^^^

On Windows, Sphinx can be install using Chocolatey. After installing Chocolatey you can run the following command in a Windows shell with administrator rights:

.. code-block:: text

   $ choco install sphinx

.. index::
   single: Linux

Linux
^^^^^

On Debian and Ubuntu, Sphinx can be install using the apt-get command. The following command will install Sphinx and Python if they are not already installed.

.. code-block:: text

   $ apt-get install python3-sphinx

Installation from source
^^^^^^^^^^^^^^^^^^^^^^^^

You can install Sphinx directly by cloning the Git repository and installing from the local clone.

.. code-block:: text

   $ git clone https://github.com/sphinx-doc/sphinx
   $ cd sphinx
   $ pip install .

If your operating system has not been mentioned, look here for additional installation instructions: https://www.sphinx-doc.org/en/master/usage/installation.html