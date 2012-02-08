The DataHub help guides. Online at http://help.thedatahub.org.

All submissions are welcome. To submit a change, fork this repo, commit your
changes, and send us a `pull request`_.

The docs are written in `ReStructured Text` format and built with Sphinx_. You
can find an introduction to Restructured Text here:
http://sphinx.pocoo.org/rest.html.

.. _ReStructured Text: http://sphinx.pocoo.org/rest.html
.. _Sphinx: http://sphinx.pocoo.org/

.. _pull request: http://help.github.com/pull-requests/


Getting Started
===============

1. Install git (or you can edit directly on github!)
2. Install sphinx - on Ubuntu do::

    apt-get install python-sphinx

You can now start editing. To build docs (e.g. to take a look at them) do::

  make html

Docs will then be in build/html


Instructions for Building Docs and Deploying
============================================

To build and deploy to http://help.thedatahub.org/::

  git checkout gh-pages
  git merge master
  make html
  ## now check to see what new html pages there are or which have been updated
  git status
  git add -u
  git add {any-new-html-pages}
  git commit -m '[build][s]: added in results of recent build.'
  ## this will initiate an automatic re-deployment to the website
  git push

