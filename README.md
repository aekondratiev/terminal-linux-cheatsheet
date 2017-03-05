From https://github.com/0nn0/terminal-mac-cheatsheet but for Linux. 

_Letters are shown capitalized for readability only._  _Capslock should be off._

# Table of Contents
1. [SHORTCUTS](#SHORTCUTS)
  1. [Terminal](#Terminal)
  2. [VIM](#VIM)
2. [CORE COMMANDS](#CORECOMMANDS)
3. [CHAINING COMMANDS](#CHAININGCOMMANDS)
4. [PIPING COMMANDS](#PIPINGCOMMANDS)
5. [COMMAND HISTORY](#COMMANDHISTORY)
6. [FILE MANAGEMENT](#FILEMANAGEMENT)
7. [DIRECTORY MANAGEMENT](#DIRECTORYMANAGEMENT)
8. [SEARCH](#SEARCH)
9. [HELP](#HELP)

## SHORTCUTS <a name="SHORTCUTS"></a>

### Terminal <a name="Terminal"></a>

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

### VIM <a name="VIM"></a>

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

## CORE COMMANDS <a name="CORECOMMANDS"></a>

| Key/Command | Description |
| ----------- | ----------- |
| cd |  Home directory |
| cd [folder] | Change directory e.g. `cd documents` |
| cd /  | Root of drive |
| cd -  | Previous directory |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh| Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| ls -ltr | Sort by creation/editing|
| sudo [command] | Run command with the security privileges of the superuser (Super User DO) |
| open [file] | Opens a file ( as if you double clicked it ) |
| top | Displays active processes. Press q to quit |
| nano [file] | Opens the file using the nano editor |
| vim [file] | Opens the file using the vim editor |
| clear |  Clear screen |
| reset |  Resets the terminal display |

## CHAINING COMMANDS <a name="CHAININGCOMMANDS"></a>

| Key/Command | Description |
| ----------- | ----------- |
| [command-a]; [command-b] | Run command A and then B, regardless of success of A |
| [command-a] && [command-b] | Run command B if A succeeded |
| [command-a] || [command-b] | Run command B if A failed |
| [command-a] & | Run command A in background |

## PIPING COMMANDS <a name="PIPINGCOMMANDS"></a>

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | Run command A and then pass the result to command B e.g ps auxwww \| grep google
|

## COMMAND HISTORY <a name="COMMANDHISTORY"></a>

| Key/Command | Description |
| ----------- | ----------- |
| history n |  Shows the stuff typed – add a number to limit the last n items |
| Ctrl + r  | Interactively search through previously typed commands |
| ![value] |  Execute the last command typed that starts with ‘value’ |
| !! |  Execute the last command typed |

## FILE MANAGEMENT <a name="FILEMANAGEMENT"></a>

| Key/Command | Description |
| ----------- | ----------- |
| touch [file] |   Create new file |
| pwd | Full path to working directory |
| . |  Current folder, e.g. `ls .` |
| .. | Parent/enclosing directory, e.g. `ls ..` |
| `ls -l ..` | Long listing of parent directory |
| `cd ../../` | Move 2 levels up |
| cat | Concatenate to screen |
| rm [file] |  Remove a file, e.g. `rm data.tmp` |
| rm -i [file] | Remove with confirmation |
| rm -r [dir] | Remove a directory and contents |
| rm -f [file] | Force removal without confirmation |
| cp [file] [newfile] | Copy file to file |
| cp [file] [dir] | Copy file to directory |
| mv [file] [new filename] |  Move/Rename, e.g. `mv file1.ad /tmp` |
| pbcopy < [file] | Copies file contents to clipboard |
| pbpaste | Paste clipboard contents |
| pbpaste > [file] | Past clipboard contents into file, `pbpaste > paste-test.txt` |

## DIRECTORY MANAGEMENT <a name="DIRECTORYMANAGEMENT"></a>

| Key/Command | Description |
| ----------- | ----------- |
| mkdir [dir] | Create new directory |
| mkdir -p [dir]/[dir] |  Create nested directories |
| rmdir [dir] | Remove directory ( only operates on empty directories ) |
| rm -R [dir] | Remove directory and contents |
| [command] \| [command] | Allows to combine multiple commands that generate output, e.g. `cat data.txt | pbcopy` |
| less |  Output content delivered in screensize chunks |
| [command] > [file] |  Push output to file, keep in mind it will get overwritten |
| [command] >> [file] | Append output to existing file |
| [command] < [file] |  Tell command to read content from a file |

## SEARCH <a name="SEARCH"></a>

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Search for files, e.g. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Search for all lines that contain the pattern, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [file] | Recursively search for all lines that do not contain the pattern |
| grep -v [search_pattern] [file] | Search for all lines that do NOT contain the pattern |

## HELP <a name="HELP"></a>

| Key/Command | Description |
| ----------- | ----------- |
| [command] -h |  Offers help |
| [command] —help | Offers help |
| info [command] | Offers help |
| man [command] |  Show the help manual for [command] |
| whatis [command] | Gives a one-line description of [command] |
| apropos [search-pattern] | Searches for command with keywords in description |
