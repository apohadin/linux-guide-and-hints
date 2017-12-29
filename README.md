# Linux Guide and Hints

[![Build Status](https://travis-ci.org/remyabel/linux-guide-and-hints.svg?branch=master)](https://travis-ci.org/remyabel/linux-guide-and-hints)

This wiki uses a forked/heavily modified version of [Sphinx RTD Theme](https://github.com/snide/sphinx_rtd_theme).

The website is live at https://www.linuxguideandhints.com

Our servers at the data center have suffered from an irrecoverable crash.
We're looking into alternative hosting.

## Copyright

The website uses the MIT license.

Primary developer: remyabel (Tommy Nguyen)

Fedora articles: remyabel

CentOS articles: [nazunalika](https://github.com/nazunalika) (Louis Abel)

### Builds

See https://travis-ci.org/remyabel/linux-guide-and-hints

### Sphinx

`pip` automatically comes with Python.

You need Sphinx in order to build this project.

    pip install --user sphinx

It will be located in `~/.local/bin/`, which you can add to your path.

Then run `make html` or `sphinx-build -Ea -b html -d build/doctrees
source build/html` from the root directory of the Sphinx project.

Alternatively, `make html SPHINXOPTS=-Ea` will achieve the same effect
in forcing an entire rebuild.

### Livereload

    npm install -g grunt-cli
    npm install
    grunt

Add `localhost.ssl` to your `/etc/hosts`, then visit `https://localhost.ssl:8443`. 
    
