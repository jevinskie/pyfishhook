========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |github-actions|
        | |coveralls| |codecov|
        | |scrutinizer| |codeclimate|
    * - package
      - | |version| |wheel| |supported-versions| |supported-implementations|
        | |commits-since|
.. |docs| image:: https://readthedocs.org/projects/pyfishhook/badge/?style=flat
    :target: https://pyfishhook.readthedocs.io/
    :alt: Documentation Status

.. |github-actions| image:: https://github.com/jevinskie/pyfishhook/actions/workflows/github-actions.yml/badge.svg
    :alt: GitHub Actions Build Status
    :target: https://github.com/jevinskie/pyfishhook/actions

.. |coveralls| image:: https://coveralls.io/repos/github/jevinskie/pyfishhook/badge.svg?branch=main
    :alt: Coverage Status
    :target: https://coveralls.io/github/jevinskie/pyfishhook?branch=main

.. |codecov| image:: https://codecov.io/gh/jevinskie/pyfishhook/branch/main/graphs/badge.svg?branch=main
    :alt: Coverage Status
    :target: https://app.codecov.io/github/jevinskie/pyfishhook

.. |codeclimate| image:: https://codeclimate.com/github/jevinskie/pyfishhook/badges/gpa.svg
   :target: https://codeclimate.com/github/jevinskie/pyfishhook
   :alt: CodeClimate Quality Status

.. |version| image:: https://img.shields.io/pypi/v/pyfishhook.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/pyfishhook

.. |wheel| image:: https://img.shields.io/pypi/wheel/pyfishhook.svg
    :alt: PyPI Wheel
    :target: https://pypi.org/project/pyfishhook

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pyfishhook.svg
    :alt: Supported versions
    :target: https://pypi.org/project/pyfishhook

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pyfishhook.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/pyfishhook

.. |commits-since| image:: https://img.shields.io/github/commits-since/jevinskie/pyfishhook/v0.1.0.svg
    :alt: Commits since latest release
    :target: https://github.com/jevinskie/pyfishhook/compare/v0.1.0...main


.. |scrutinizer| image:: https://img.shields.io/scrutinizer/quality/g/jevinskie/pyfishhook/main.svg
    :alt: Scrutinizer Status
    :target: https://scrutinizer-ci.com/g/jevinskie/pyfishhook/


.. end-badges

Python bindings and bundled build of fishhook: A library that enables dynamically rebinding symbols in Mach-O binaries
running on  macOS/iOSS.

* Free software: BSD 3-Clause License

Installation
============

::

    pip install pyfishhook

You can also install the in-development version with::

    pip install https://github.com/jevinskie/pyfishhook/archive/main.zip


Documentation
=============


https://pyfishhook.readthedocs.io/


Development
===========

To run all the tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOPTS=--cov-append
            tox

    - - Other
      - ::

            PYTEST_ADDOPTS=--cov-append tox
