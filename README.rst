leocornus.buildout.cfgrepo
==========================

Create this repository to save some buildout configuration files
to make my daily development work easier.

What's in
=========

I will try to include the following utilities:

 * MySQL database compile and build
 * MySQL database server setup utilities
 * SQLite3 compile and build
 * Nginx compile and build
 * Nginx database server setup utilities.
 * Magento webshop installation

How to use
==========

cfgrepo is very easy to use.  You could try the following methods:

 * hard copy, download from GitHub and copy to your buildout facility.
 * symlink, clone from GitHub and symlink to your buildout folder.
 * submodule, adding cfgrepo as a submodule of your project.

git submodule and tag
=====================

Add cfgrepo as a submodule

$ cd myproject
$ git submodule add git://github.com/leocornus/leocornus.buildout.cfgrepo.git buildout/cfgrepo
$ git commit -m "add cfgrepo as submodule" .

Update to use a certian tag.

$ cd buildout/cfgrepo
$ git checkout v0.1
$ cd ../..
$ git add buildout/cfgrepo
$ git commit -m "update to cfgrepo v0.1" buildout/cfgrepo
$ git push

Register and update submodule in your project.

$ cd myproject
$ git submodule init
$ git submodule update

License
=======

GNU General Public License Version 2

Change Log
==========

0.3 (NO Release)
----------------

 - Alternative way to setup supervisor by using
   collective.recipe.template and zc.recipe.egg.

0.2 (2012-05-08)
----------------

 - Add config profile to build legacy MySQL database server
   up to version 5.1.x

0.1 (2012-04-27)
----------------

 - initial release, taged as v0.1
