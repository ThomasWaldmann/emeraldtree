Change Log
==========

Version 0.12.0 (2026-03-06)
---------------------------

New features:

- improved XPath support:

  - support .// and ..
  - support [position]

Other changes:

- support Python 3.13 and 3.14, drop support for Python 3.9
- switch to SPDX license identifier
- use native ``pyproject.toml`` support in tox
- add scripts for sdist, signing, and PyPI upload

Version 0.11.0 (2024-04-05)
---------------------------

Fixes:

- HTML parser: fix extraction of encoding from meta element
- use raw string for regex, fixes "DeprecationWarning: invalid escape
  sequence \s" and others.

New features:

- include version info into emeraldtree.__init__

Other changes:

- packaging modernized / enhanced: pyproject.toml, MANIFEST.in, setuptools-scm
- requires Python >= 3.9 now (dropped Python 2.x, removed "six")
- add GitHub Actions CI, remove Travis CI config
- rst markup fixes / cleanups
- use tox for testing

Version 0.10.0 (2015-06-10)
---------------------------

Fixes:

- fix setup.py - platform and no download_url
- fix invalid output from HTML converter parsing preformatted code, multiline
  paragraphs: part 2 of 2 fixes moin2 #516

Other changes:

- ported to Python 2.7 / >= 3.3 using six

Version 0.9.0 (2011-01-22)
--------------------------

First release on PyPI.

