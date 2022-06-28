CommandManager
===============

Class file location: :file:`core/CommandManager/index.js`

.. js:function:: registerCommand(commandName, handler)

    Register command

    :static:
    :param string commandName: Name of command (for example "help")
    :param string handler: Command handler [1]_

.. js:function:: unregisterCommand(commandName)

    Unregister command

    :static:
    :param string commandName: Name of command

.. js:function:: listCommands()

    List all registered commands

    :static:
    :return: string[]

.. js:function:: hasCommand(commandName)

    Check if command registered

    :static:
    :param string commandName: Name of command
    :return: boolean

.. js:function:: isDisabled(commandName)

    Check if command disabled

    :static:
    :param string commandName: Name of command
    :return: boolean

.. js:function:: disableCommand(commandName)

    Disable command

    :static:
    :param string commandName: Name of command

.. js:function:: enableCommand(commandName)

    Enable command

    :static:
    :param string commandName: Name of command

.. js:function:: getEventManager()

    Gives event manager

    :ref:`List of supported events <commandManager/events>`

-----------------------------------------------------------------------------------------------------------------------

.. [1]

    .. js:function:: handler(args, message)

        :param string[] args: Command args splited by `splitargs <https://www.npmjs.com/package/splitargs>`_
        :param Message message: Raw `message <https://discord.js.org/#/docs/discord.js/13.6.0/class/Message>`_ object

-----------------------------------------------------------------------------------------------------------------------

Events
------

.. _commandManager/events:

.. _commandManager/commandRegisteredEvent:

commandRegistered
    Emit when command registered

    :params: (commandName)

.. _commandManager/commandUnregisteredEvent:

commandUnregistered
    Emit when command unregistered

    :params: (commandName)

.. _commandManager/commandDisabledEvent:

commandDisabledEvent
    Emit when command disabled

    :params: (commandName)

.. _commandManager/commandEnabledEvent:

commandEnabledEvent
    Emit when command enabled

    :params: (commandName)
