CliModule
=========

System module that provide CLI.

Instance can be taken via :js:func:`ModuleManager.getModule(name)<getModule>`

.. js:function:: addCommand(command, commandHandler [, commandCompleter])

    Add command with specified handler and completer.

    .. warning:: **ALL** command handlers will execute. By that reason you should check command in your handler

    :param string command: Command name
    :param function commandHandler: Command handler [1]_
    :param function commandCompleter: Command completer [2]_
    :return: boolean

.. js:function:: removeCommand(command)

    Remove registered command

    :param string command: Command name
    :return: boolean

.. js:function:: pauseCli()

    This function used to pause CLI input  after executing command that can take long time.

.. js:function:: resumeCli()

    Resume CLI input after job done.

------------------------------------------------------------------------------

.. [1] .. js:function:: commandHandler(input)
        :param string input: Entered string (example: "shutdown")

.. [2] .. js:function:: commandCompleter(line)
        :param string line: Entered line (example: "shut")
        :return: string[]|null
            Array of hits or null if none fit.
            Hit must be full command

            :example: ["shutdown"]