Core
=====

.. _DiscordClient: https://discord.js.org/#/docs/discord.js/13.6.0/class/Client

Class file location: :file:`core/core.js`

.. js:function:: init()

    Function for initialize core.

.. js:function:: getCore()

   Core instance getter

    :return: :doc:`Core <core>`

.. js:function:: getConfig()

    Returns config

    :return: :ref:`Config <configuration>`

.. js:function:: getClient()

    Return Discord.js client

    :return: `DiscordClient`_

.. js:function:: shutdown()

    Unloads all modules and exit process

.. js:function:: getModuleManager()

    Return module manager instance.

    :return: :doc:`ModuleManager <moduleManager>`

.. js:function:: getCommandManager()

    Return command manager instance.

    :return: :doc:`CommandManager <commandManager>`

.. js:function:: getLogger()

    Return logger.

    :return: :doc:`Logger <Logger>`

.. js:function:: registerClientEvent(type, handler[, once = false])

    Register event in `DiscordClient`_

    :param string type:
    :param handler: Event handler callback
    :param boolean once: If true register once event
    :return: UUID of registered event

.. js:function:: unregisterClientEvent(uuid)

    :param string uuid: UUID of event listener