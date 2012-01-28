The DataHub help guides. Online at http://help.thedatahub.org.

All submissions are welcome. To submit a change, fork this repo, commit your
changes, and send us a `pull request`_.

.. _pull request: http://help.github.com/pull-requests/

Instructions for Use
====================

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

