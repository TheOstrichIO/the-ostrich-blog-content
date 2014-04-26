When working on my Windows laptop,
I often find myself needing to launch a new command prompt,
usually in a specific folder
(e.g., the active folder in Windows Explorer,
or in my favorite file manager on Windows- Total Commander).

This happens often enough that I decided to use AutoHotKey
(the awesome Windows automation tool)
to create a keyboard shortcut to automate the process.

Properties and features of the AHK script I came up with:

- Invoked with a keyboard shortcut Ctrl+Alt+T
  (so it's consistent with launching the terminal in Linux).
- If in Windows Explorer -
  start the command prompt in the current folder.
- If in Total Commander -
  start the command prompt in the current folder of the active pane.
- Otherwise, use a default folder (e.g., the home folder).

The code:

https://gist.github.com/itamaro/6328491
