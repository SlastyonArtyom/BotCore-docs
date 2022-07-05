Usage
=====

.. _installation:

Installation
------------

To install BotCore in current directory, run this command:

.. code-block:: console

    $ wget -O - https://tenorium.github.io/BotCore-install/install.js | node

.. _configuration:

Configuration
--------------

Main config file is :file:`config/core.config.js`

Config fields:

.. _loggerOptions:

logger
    Logger options.

    debug
        :type: Boolean
        Enable debug mode
    dateformat
        :type: String
        Compatible with `moment.js <https://momentjs.com/docs/#/displaying/format/>`_ date format
client
    `Options <https://discord.js.org/#/docs/discord.js/13.6.0/typedef/ClientOptions>`_ for Discord.JS client
locale
    :values: "ru","en"
    Locale used by botcore.
token
    Discord bot token
prefix
    Prefix for commands

Starting
--------

For start bot run next command:

.. code-block:: console

    $ npm run bot

After starting you can see logs and :doc:`cli` prompt.
