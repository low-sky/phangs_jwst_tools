phangs jwst tools
-----------------

.. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
    :target: http://www.astropy.org
    :alt: Powered by Astropy Badge


License
-------

This project is Copyright (c) PHANGS team and licensed under
the terms of the GNU GPL v3+ license. This package is based upon
the `Astropy package template <https://github.com/astropy/package-template>`_
which is licensed under the BSD 3-clause license. See the licenses folder for
more information.


Quick Start
-----------

This package provides tools for working with JWST data in the PHANGS project.

**False source injection**

The `complim` module handles false source injection and measurement of completeness limits for JWST lv3 images.  There are two primary modes for using the module.  Just running the `completeness_limit` module on a filename performing the completeness analysis and returns a 99% completeness limit by default using the `IRAFStarFinder` in `photutils` with optional diffuse emission filtering using the constrained diffusion algorithm. Using the `write_fake_files` will build a library of images with fake files included. The `completeness_analysis` module compares a photometric catalog generated by external source identification routine to the sources in a library of false-source files to determine the completeness limit. The `completeness_analysis` module will return the 99% completeness limit by default.

