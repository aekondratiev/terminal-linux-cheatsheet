From https://github.com/0nn0/terminal-mac-cheatsheet but for Linux. 

_Letters are shown capitalized for readability only._  _Capslock should be off._
## SHORTCUTS

### Terminal

| Key/Command | Description |
| ----------- | ----------- |
| Ctrl + A   | Go to the beginning of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + E   | Go to the end of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + L   | Clears the Screen |
| Ctrl + U   | Cut everything backwards to beginning of line |
| Ctrl + K   | Cut everything forward to end of line |
| Ctrl + W   | Cut one word backwards using white space as delimiter |
| Ctrl + Y   | Paste whatever was cut by the last cut command |
| Ctrl + H   | Same as backspace |
| Ctrl + C   | Kill whatever you are running |
| Ctrl + D   | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z   | Puts whatever you are running into a suspended background process. fg restores it. |
| Ctrl + _   | Undo the last command. (Underscore.  So it's actually Ctrl + Shift + minus) |
| Ctrl + T   | Swap the last two characters before the cursor |
| Ctrl + F   | Move cursor one character forward |
| Ctrl + B   | Move cursor one character backward |
| Tab  | Auto-complete files and folder names |

### VIM

| Key/Command | Description |
| ----------- | ----------- |
| u | undo |
| Ctrl + r | redo |
| gg | go to the first line of the document |
| G | go to the last line of the document |
| } | jump to next paragraph (or function/block, when editing code) |
| { | jump to previous paragraph (or function/block, when editing code) |
| Ctrl + b | move back one full screen |
| Ctrl + f | move forward one full screen |
| v | start visual mode, mark lines, then do a command (like y-yank) |
| Esc | exit visual mode |
| yy | yank (copy) a line |
| p | put (paste) the clipboard after cursor |
| P | put (paste) before cursor |
| dd | delete (cut) a line |
| D | delete (cut) to the end of the line |
| x | delete (cut) character |
| i | insert before the cursor |
| I | insert at the beginning of the line |
| a | insert (append) after the cursor |
| A | insert (append) at the end of the line |
| o | append (open) a new line below the current line |
| O | append (open) a new line above the current line |
| :%s/old/new/g | replace all old with new throughout file |
| :%s/old/new/gc | replace all old with new throughout file with confirmations |
