Module
======

All modules located in :file:`modules` folder

For every module in :file:`modules` folder must be created with name of module and module main file.

:Example: :file:`modules/{moduleName}/{moduleName}.js`

.. warning:: Module file must be ES6 module!

You should:

* add default export of class that extends :doc:`AbstractModule <../api/abstractModule>`
* implement load function