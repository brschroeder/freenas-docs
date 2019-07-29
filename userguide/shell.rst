.. index:: Shell
.. _Shell:

Shell
=====

Beginning with version 8.2.0, the %brand% |web-ui| provides a web shell,
making it convenient to run command line tools from the web browser as
the *root* user.

.. _web_shell_fig:

.. figure:: images/shell.png

   Web Shell


The prompt shows that the current user is *root*, the hostname is
*freenas*, and the current working directory is :file:`~`, the home
directory of the logged-in user.

.. note:: The default shell for a new install of %brand% is
   `zsh <https://www.freebsd.org/cgi/man.cgi?query=zsh>`__.
   %brand% systems which have been upgraded from an earlier
   version will continue to use :command:`csh` as the default shell.

   The default shell can be changed in
   :menuselection:`Accounts --> Users`.
   Click |ui-options| and :guilabel:`Edit` for the *root* user. Choose
   the desired shell from the :guilabel:`Shell` drop-down and click
   :guilabel:`SAVE`.


The :guilabel:`Set font size` slider adjusts the size of text
displayed in the Shell. Click :guilabel:`RESTORE DEFAULT` to reset the
shell font and size.

A history of previous commands is available. Use the up and down arrow
keys to scroll through previously entered commands. Edit the command if
desired, then press :kbd:`Enter` to re-enter the command.

:kbd:`Home`, :kbd:`End`, and :kbd:`Delete` keys are supported. Tab
completion is also available. Type a few letters and press :kbd:`Tab` to
complete a command name or filename in the current directory. Right-
clicking in the terminal window displays a reminder about
using :kbd:`Command+c` and :kbd:`Command+v` or :kbd:`Ctrl+Insert` and
:kbd:`Shift+Insert` for copy and paste operations in the %brand% shell.

Type :command:`exit` to leave the session.

Clicking other |web-ui| menus closes the shell session and stops
commands running in the shell. :ref:`tmux` provides the ability
to detach shell sessions and then reattach to them later. Commands
continue to run in a detached session.

.. note:: Not all shell features render correctly in Chrome. Firefox
   is the recommended browser when using the shell.


Most FreeBSD :ref:`command line utilities <Command Line Utilities>` are
available in the :guilabel:`Shell`, including additional troubleshooting
applications for %brand%.
