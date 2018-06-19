====================
plonetheme.evergreen
====================


Introduction
============

*plonetheme.evergreen* package is an installable Plone_ Theme using the **theming** and **packaging** 
features available in `plone.app.theming`_ to make the theme `evergreen`_ easily
available in `Plone`.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest versión (https://plone.org/download)
- The ``plone.app.theming`` package (*will be installed as a dependency of this package*)


Features
========

- It's an installable Plone_ Theme package.
- After installation from Add-ons controlpanel, this theme is enabled automatically.
- Also it's a simple Diazo_ package (Zip file).
- It's have support for clean uninstallation.


Installation
============


Add Plone site
--------------

Install Plone 4.x with `plone.app.theming`_ and create a Plone site (if you have not already)
with Diazo theming configured.

.. image:: https://github.com/collective/plonetheme.evergreen/raw/master/screenshot0.png
  :width: 1024px
  :alt: Create a Plone site from ZMI
  :align: center


Zip file
--------

If you are an **end user**, you might enjoy installation via zip file import.

1. Download a `zip file <https://raw.github.com/collective/plonetheme.evergreen/master/evergreen.zip>`_.
2. Import the theme from the Diazo theme control panel.

.. image:: https://github.com/collective/plonetheme.evergreen/raw/master/screenshot1.png
  :width: 1024px
  :alt: Import the Diazo theme zip file
  :align: center


Buildout
--------

If you are a **developer user**, you might enjoy installing it via buildout.

For install ``plonetheme.evergreen`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        plonetheme.evergreen


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'plonetheme.evergreen',
    ],


Enabling the theme
^^^^^^^^^^^^^^^^^^

Browse to ``http://yoursite/Plone/@@theming-controlpanel`` click on ``Enable`` 
on ``Evergreen`` theme from the Diazo control panel.

.. image:: https://github.com/collective/plonetheme.evergreen/raw/master/screenshot2.png
  :width: 1024px
  :alt: For select the Diazo theme just click on Activate button
  :align: center

That's it!

You should see the layout of the site when viewed in a computer resolution:

.. image:: https://raw.githubusercontent.com/collective/plonetheme.evergreen/master/plonetheme/evergreen/static/preview.png
    :align: center


Contribute
==========

- Issue Tracker: https://github.com/collective/plonetheme.evergreen/issues
- Source Code: https://github.com/collective/plonetheme.evergreen


License
=======

This package is licensed under the GPL Version 2.


Credits
-------

- Giacomo Spettoli (giacomo.spettoli at gmail dot com).
- Leonardo J. Caballero G. (leonardocaballero at gmail dot com).

.. _`Plone`: http://plone.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`evergreen`: http://www.freecsstemplates.org/preview/evergreen/
.. _`Diazo`: http://diazo.org
