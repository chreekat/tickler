tickler, a low-tech digital implementation of the tickler concept of GTD and
43-folder fame.

tickler is implemented as a bash script, so it should work wherever bash works.
I guess. Well, it also uses other standard Linux utilities, e.g. stat, so I guess
this is a Linux app.

CONCEPT
======

The idea is to use directories to represent the 43 folders. Shuffling the
folders is handled for you. Folders that aren't empty are highlighted.

USAGE
====

First of all
-----------

1. Specify the "file cabinet", i.e. the directory the folders are rooted in, by
modifying the proper variable within the script.

    ```bash
    # This is where all the tickler directories physically live. Modify to taste.
    Filing_cabinet=~/Org/Reference/Tickler
    ```
2. Copy bashrc to your file cabinet.

And then
--------

* When you select a folder, you are dropped to a shell with the PWD set to the
  proper directory. Suggestions: Add a TODO file! Copy those meetings notes
  over! Whatever!
* If today's folder isn't empty, open that bad boy up and copy the TODO contents
  to your organizer. Or whatever.

Like I said, low-tech.
