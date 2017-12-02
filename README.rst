================================================
Sublime Text Java Bytecode (Syntax highlighting)
================================================

.. image:: https://img.shields.io/badge/package-control-blue.svg?style=plastic
   :target: https://packagecontrol.io/packages/Java%20Bytecode

Overview
========

This is a package for introducing Java bytecode syntax highlighting to the `Sublime Text  <http://www.sublimetext.com/>`_
editor (*ST2/ST3*). 

Currently supported:

- `Javap <http://docs.oracle.com/javase/7/docs/technotes/tools/windows/javap.html>`_ output
- `Java Bytecode Editor <http://set.ee/jbe/>`_ output


Javap (Java class file disassembler)
*************************************


.. image:: http://i.imgur.com/QbtbKpg.png


JBE (Java Bytecode Editor)
********************************
.. image:: http://i.imgur.com/uAXOxfy.png



Version
=======

1.0.5

Installation
=============


#. Having installed `Package Control <https://packagecontrol.io/installation>`_ access the ``Command Pallete`` (`Ctrl+Shift+P`), select ``Install package`` and then select ``Java Bytecode``.

#. In the bottom right corner click and select **Java Bytecode > Java Bytecode (Default)** (or `Custom` if you've set up a custom color scheme)


*Alternatively* if you have not installed Package control (which I highly recommend):

#. Go to **Preferences | Browse packages...**
#. While inside the **Packages** directory, clone the theme repository using the command below: 

    ``git clone https://github.com/xdrop/Java-Bytecode.git "Java Bytecode"``




Custom syntax highlighting
===========================
The package comes with support for custom syntax highlighting by including the following custom scopes:

* ``return`` and similar keywords
* ``new`` keyword
* ``getfield/putfield`` and similar field accessors
* ``astore`` and similar local field storing
* ``aload`` and similar local field loaders
* calls to ``invoke...`` 
* ``nop``
* java keywords used by javap
* list of all bytecode instructions

**(!)** To use custom syntax coloring you need to edit the theme you use to provide support for these custom scopes.

Instructions
*************
#. Obtain the ``.tmTheme`` file of the color scheme you are using and wish to edit
#. Open it in a text editor
#. Get the ``addedscopes.xml`` file from this package directory
#. Locate the ``</array>`` closing tag and copy the contents of ``addedscopes.xml`` **before** it.
#. Load your new ``.tmTheme`` file into `tmTheme Editor  <https://github.com/aziz/tmTheme-Editor>`_ and customize it to your needs.
#. Download it and add it to your packages directory.
#. Go to **Preferences | Color Scheme** and select it.
#. Set **Java Bytecode (Custom highlighting)** as your language.


License:
==========

Copyright (c) 2015-2017 xdrop


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:


The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.


THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
