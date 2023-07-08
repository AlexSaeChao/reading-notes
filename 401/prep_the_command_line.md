# The Command Line - Prep Work

## Intro - Command Line

In the Introduction in Ryan's Tutorial, They talk about what the command line, aka terminal, being a text based interface to the system.

In the terminal to look at what is in the directory or file you could use `ls` to see which files and directories are there in the current directory you're in. You could add a command line argument (`ls -l`) to have optional behaviour.

## Navigation

`pwd` lets you see where you're located by showing you your current directory and the path to your location.

What's in the current location, use `ls` to show what is there.

Absolute and Relative Paths talk about where a file or directory is located in relation to the root directory (absolute) or from your current location (relative)

Absolute path is denoted with a `/` at the beginning of the path and its subdirectories after.

`cd` is used to change your directory followed by the path of your file or directory.

## More About Files

Everything is a file. For example your keyboard is a file that is read only by the system. everything under the hood is a file.

Linux is case sensitive, watch and be cautious about how you name your files.

If a file's name has a space to break the name you need single quotes when calling to it when refering to it in file paths or naming it directly.

You could also use a `\` to nullify the special meaning of the next character.

`ls -a` lists the contents of the directory, including hidden files.

## Manual Pages

Manual pages is basically looking up the manual for a command, for example you can you `man ls` in the terminal to see how `ls`  works and what other arguments it may have.

You could use `man -k <search term>` to search for key words in the manual.

``` terminal

/<term>
<!-- Within a manual page, perform a search for 'term' -->
n
<!-- After performing a search within a manual page, select the next found item. -->

```

With these terminal commands you can make files and folders and name them right after the command followed by a space.

Be careful when deleting files and directories because they are permanent actions

``` terminal

mkdir
<!-- Make Directory - ie. Create a directory. -->
rmdir
<!-- Remove Directory - ie. Delete a directory. -->
touch
<!-- Create a blank file. -->
cp
<!-- Copy - ie. Copy a file or directory. -->
mv
<!-- Move - ie. Move a file or directory (can also be used to rename). -->
rm
<!-- Remove - ie. Delete a file. -->
No undo
<!-- The Linux command line does not have an undo feature. Perform destructive actions carefully. -->
Command line options
<!-- Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available. -->

```

### References

[Ryan's Tutorials](https://ryanstutorials.net/linuxtutorial/)

[Ryan's Tutorials - Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php)

[Ryan's Tutorials - Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php)

[Ryan's Tutorials - More about Files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php)

[Ryan's Tutorials - Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php)

[Ryan's Tutorials - File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php)

[Ryan's Tutorials - Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)
