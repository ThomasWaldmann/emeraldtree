EmeraldTree, a light-weight toolkit for XML processing
======================================================

EmeraldTree is a fork of ElementTree - the main differences are:

* It has a slightly different API for handling of text: it uses
  unicode objects as children (not as "tail" attributes of the elements)
* API cleanups, removing backward compatibility
* Better unicode support
* PolyglotWriter (for writing html5 that is also well-formed xml)
* Other improvements / optimizations

The fork happened at ElementTree 1.3a3-20070912-preview, for more details
please see the repositories:

* https://github.com/moinwiki/emeraldtree/
* http://svn.effbot.org/public/elementtree-1.3/

Changes are (c) by their authors (see also source files) and licensed
under the same Python (MIT style) license as ElementTree (see below):

* Bastian Blank <bblank@thinkmo.de>


Here is the original README contents of ElementTree:

=======================
The elementtree library
=======================

This kit contains the ElementTree library, a light-weight toolkit for
XML processing in Python.

For more information on this library, see:

* docs/index.html
* http://effbot.org/zone/element.htm

The 1.3 release is designed to work with Python 2.2 and newer.  If you
need support for earlier Python releases, use ElementTree 1.2.6.

Enjoy /F

fredrik@pythonware.com
http://www.pythonware.com

--------------------------------------------------------------------
release info
--------------------------------------------------------------------

This is release 1.3 alpha 3 of the ElementTree library.

For a list of changes in this release, see the CHANGES document.

The latest version of this library can be downloaded from:

http://effbot.org/downloads

Comments, bug reports, and patches are welcome.  Send them to
fredrik@pythonware.com.

Note that this is free software, with limited support.  If you need
commercial support on this module, contact fredrik@pythonware.com.

--------------------------------------------------------------------
contents
--------------------------------------------------------------------

 README                        This file

 CHANGES                       List of changes in this release.

 elementtree/

  ElementTree.py              Element tree implementation.  For a minimal
                              install, this file is all you need.

  ElementPath.py              Element path support module.  Adds limited
                              XPath support to find/findtext/findall.

  ElementInclude.py           Element include support module.  Adds limited
                              XInclude support.

  HTMLTreeBuilder.py          Element tree builder for HTML.  This only
                              works for mostly well-formed HTML; if you
                              need something that can parse arbitrary
                              HTML at least as good as your browser, use
                              TidyHTMLTreeBuilder or TidyTools (see below).

  TidyHTMLTreeBuilder.py      Element tree builder for HTML, based on the
                              tidylib library.  This tree builder requires
                              the _elementtidy extension module (available
                              from http://effbot.org/downloads).

  SimpleXMLWriter.py          Simple XML writer

  TidyTools.py                Build element trees from HTML, using the
                              external 'tidy' utility.

 setup.py                      Build/installation script

 docs/index.html		      API reference pages.
 docs/*

 demo*.py                      Sample scripts
 samples/*                     Sample data

 selftest.py                   Selftest (requires Python 2.1 or later)
 tidytest.py                   Selftest for TidyHTMLTreeBuilder components.

 benchmark.py                  Benchmark script (usage: benchmark.py file)

--------------------------------------------------------------------
license
--------------------------------------------------------------------

The ElementTree Library is

Copyright (c) 1999-2007 by Secret Labs AB
Copyright (c) 1999-2007 by Fredrik Lundh

By obtaining, using, and/or copying this software and/or its
associated documentation, you agree that you have read, understood,
and will comply with the following terms and conditions:

Permission to use, copy, modify, and distribute this software and its
associated documentation for any purpose and without fee is hereby
granted, provided that the above copyright notice appears in all
copies, and that both that copyright notice and this permission notice
appear in supporting documentation, and that the name of Secret Labs
AB or the author not be used in advertising or publicity pertaining to
distribution of the software without specific, written prior
permission.

SECRET LABS AB AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO
THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
FITNESS.  IN NO EVENT SHALL SECRET LABS AB OR THE AUTHOR BE LIABLE FOR
ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
