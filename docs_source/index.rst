Welcome to mer's documentation!
===============================
Mars-Earth retimer (mer) is a package for converting between Martian times and
Earth times. You may be interested in this package if:

* you're sick of people's logic-defying insistence to refer to Martian events
  in Earth times, so you want a way to convert Earth times to Martian times
  (who cares that a dust storm started April 10---a date that provides
  absolutely no physically relevant info---you just want to know the
  L\ :sub:`s` when it started), or
* you think in Martian times and begrudgingly have to give Earth dates and/or
  times to others.

If either of these apply to you, this package is for you.

A note about accuracy
---------------------
This package makes 2 assumptions that can introduce errors:

* A Mars year has a constant length. The Piqueux *et al* paper of accurate
  Mars year starting dates indicates, for example, that Mars year 97 to 98
  is 686.995 days, whereas Mars year 99 to 100 is 686.959 days. I assume the
  Mars years have a constant length, but this assumption is not quite true.
* The constants are infinitely precise. Some constants (like the solar
  longitude at perihelion) aren't particularly precise. It may not even be
  possible for them to be more precise without running into errors described in
  the first bullet point.

Therefore I recommend you use this package as a *generally* accurate
retimer---not a *supremely* accurate retimer. If you need second or minute
accuracy and precision, I suggest you use SPICE.

If you know of a way to perform more accurate calculations, please
`raise an issue <https://github.com/kconnour/mer/issues>`_ to help improve
this package.

.. toctree::
   :maxdepth: 1
   :caption: Useful links

   install
   api-reference
