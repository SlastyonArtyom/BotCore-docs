ModuleManager
=============

Class file location: :file:`core/ModuleManager/index.js`

.. js:function:: autoload()

    Load all modules

    :async:
    :static:

.. js:function:: load(name)

    Load module by name

    :async:
    :static:
    :param string name: Name of module
    :return: boolean

.. js:function:: unload(name)

    Unload module by name

    :static:
    :param string name: Name of module

.. js:function:: list()

    List all available modules

    :static:
    :return: string[]

.. js:function:: listLoaded()

    List all loaded modules

    :static
    :return: string[]

.. js:function:: getModule(name)

    Get loaded module instance by module name

    :static:
    :param string name: Name of module
    :return: :doc:`AbstractModule <abstractModule>`

.. js:function:: unloadAll()

    Unload **ALL** modules

    :static:

.. js:function:: getEventManager()

    Gives event manager.

    :ref:`List of supported events <moduleManager/events>`

    :static:

Events
------

.. _moduleManager/events:

.. _moduleManager/moduleLoadedEvent:

moduleLoaded
    Emit when module loaded

    :params: (moduleName)

        moduleName
            Name of loaded module

.. _moduleManager/moduleUnloadedEvent:

moduleUnloaded
    Emit when module unloaded

    :params: (moduleName)

        moduleName
            Name of unloaded module

.. _moduleManager/autoLoadFinished:

autoLoadFinished
    Emit when modules autoload finished