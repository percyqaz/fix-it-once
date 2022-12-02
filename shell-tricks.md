`cmd /k` will start a command prompt, finish running the command and then remain open as a normal command prompt

`cmd /c` will wrap a command that wants to force-close the terminal when done (I'm looking at node) so that the rest of the .bat file can execute
