CLI
====

BotCore have CLI for interaction with bot and correct shutdown.

.. _defaultCommands:

Default Commands
-----------------

CLI have some default commands.
Below you can see table with default commands

+---------------+----------------------------------------+---------------------------------+
| Command name  | Command description                    | Command usage                   |
+===============+========================================+=================================+
|shutdown       |This command unloads all modules        |shutdown                         |
|               |and performs shutdown                   |                                 |
+---------------+----------------------------------------+---------------------------------+
|command        |Manage commands (activate or deactivate)|command <subcommand> [1]_ [args] |
|               |                                        |                                 |
+---------------+----------------------------------------+---------------------------------+
|pkg            |Manage packages                         |pkg <subcommand> [2]_ [args]     |
+---------------+----------------------------------------+---------------------------------+

.. [1] Subcommands of command ``command``

    +-----------+-----------------------------+-----------------+
    | Subcommand| Description                 | Usage           |
    +===========+=============================+=================+
    | list      | List all registered commands| list            |
    +-----------+-----------------------------+-----------------+
    | enable    | Enable specified command    | enable <command>|
    +-----------+-----------------------------+-----------------+
    | disable   | Disable specified command   |disable <command>|
    +-----------+-----------------------------+-----------------+

.. [2] Subcommands of command ``pkg`` specified in :ref:`pkgCommands`