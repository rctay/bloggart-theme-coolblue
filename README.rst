===============================================
styleshout.com's coolblue template for bloggart
===============================================

Description
-----------

This is the `coolblue template`_ from `styleshout.com`_, modified for bloggart.
It relies on the "default" template in `bloggart`_ and overrides a few templates
here and there.

As the original coolblue template was distributed under `CC Attribution`_, this
project should also fall under it too.

.. _`bloggart`: http://github.com/Arachnid/bloggart
.. _`CC Attribution`: http://creativecommons.org/licenses/by/2.5/
.. _`coolblue template`: http://www.styleshout.com/templates/preview/CoolBlue10/index.html
.. _`styleshout.com`: http://www.styleshout.com/

Usage
-----

#. At the root of your bloggart clone, run::

     $ git submodule add git://github.com/rctay/bloggart-theme-coolblue.git themes/coolblue

   This theme tracks the `rc/master`_ branch in `my bloggart fork`_ very closely,
   and the branches here corresponds to branches there. Therefore, if your
   bloggart setup uses my branches, you should specify the branch to the
   `git submodule add` command. For example::

     $ git submodule add -b rc/master git://github.com/rctay/bloggart-theme-coolblue.git themes/coolblue

#. Modify your ``config.py``::

     diff --git a/config.py b/config.py
     index dab53cb..b0d4e27 100644
     --- a/config.py
     +++ b/config.py
     @@ -15,7 +15,7 @@ host = 'localhost:8080'

      # Selects the theme to use. Theme names correspond to directories under
      # the 'themes' directory, containing templates and static content.
     -theme = 'default'
     +theme = 'coolblue'

      # Defines the URL organization to use for blog postings. Valid substitutions:
      #   slug - the identifier for the post, derived from the title

#. If you've already posted posts in your previous theme, you will have to
   regenerate them for the coolblue theme to take effect.

.. _`rc/master`: http://github.com/rctay/bloggart/tree/rc/master
.. _`my bloggart fork`: http://github.com/rctay/bloggart
