===============================================
styleshout.com's coolblue template for bloggart
===============================================

Description
-----------

This is the `coolblue template`_ from `styleshout.com`_, modified for bloggart,
based on a fork of the "default" template in `bloggart`_.

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

   If you've merged in my `configurable defer feature`_, then this should read::

     $ git submodule add -b rc/defer-config git://github.com/rctay/bloggart-theme-coolblue.git themes/coolblue

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

.. _`configurable defer feature`: http://github.com/rctay/bloggart/tree/rc/defer-config
