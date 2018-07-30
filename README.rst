Tanya's blog
============

This is blog uses Nikola_ with a custom theme.
The instructions for deployment are pretty straightforward;
the primary branch you edit in is called `src`, and the
shell command `nikola github_deploy` will automate deployment
to the main branch.

The theming was not as straightforward, but I copied and modified the
base theme in
`themes/custom<https://github.com/tanyaschlusser/tanyaschlusser.github.io/tree/src/themes/custom>`_,
removing the baguette and other javascript tools for image libraries
and slideshows; and the library that was used for responsive layout.
(I think these things can be handled now with modern HTML and CSS).
I replaced the KaTeX_ library with the newest version (10.0 beta),
even though it's beta now, because I otherwise can't see the horizontal
line in display fractions. Looks great as far as I can tell;
thanks Khan academy!

Feel free to copy the CSS and theme, with the caveat
that I didn't make it extensible, and may have hard-coded
my own URLs.


.. _Nikola: https://getnikola.com/
.. _KaTeX: https://khan.github.io/KaTeX/
