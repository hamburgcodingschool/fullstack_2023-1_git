# Command Line Cheat Sheet

This cheat sheet is for using the Terminal (bash) on MacOS.

## Files and Folders

List all the files on your current location:
```
ls
```

List all the files, one per line, with some more information:
```
ls -al
```

Go into a folder:
```
cd <folder name>
```

Go into a folder in a folder in a folder...
```
cd <path/to/your/folder>
```

Create a new folder:
```
mkdir folder_name
```

Create a new file:
```
touch file_name.txt
```

Delete a file:
```
rm file_name.txt
```

Delete a folder and all its contents:
```
rm -rf folder_name
```

## Tipps and Tricks

Clear the command line:
```
clear
```

Repeat a previous command: `⬆️ arrow up`

See a whole bunch of your last commands:
```
history
```

Execute a command from the history:
```
!<number of the command>
```

Autocomplete: `tab`

Show the whole path where you are right now:
```
pwd
```

Show the whole path of where a file is:
```
realpath file.txt
```
> If this doesn't work, you need to install `coreutils`:
>
> `brew install coreutils`
