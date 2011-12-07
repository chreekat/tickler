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

* Run tickler. You get a menu to select folders:

    ```
    $ tickler

    ** Using /home/b/Org/Reference/Tickler as filing cabinet.

     1) Dec-07              16) Dec-22              31) Jan-05
     2) Dec-08 (tomorrow)   17) Dec-23              32) Jan-06
     3) Dec-09 (Fri)        18) Dec-24              33) February
     4) Dec-10 (Sat)        19) Dec-25              34) March !!
     5) Dec-11 (Sun)        20) Dec-26              35) April
     6) Dec-12 (Mon)        21) Dec-27              36) May
     7) Dec-13 (Tue)        22) Dec-28              37) June
     8) Dec-14 (next week)  23) Dec-29              38) July
     9) Dec-15              24) Dec-30              39) August
    10) Dec-16              25) Dec-31              40) September
    11) Dec-17              26) January             41) October
    12) Dec-18              27) Jan-01              42) November
    13) Dec-19              28) Jan-02              43) December
    14) Dec-20              29) Jan-03
    15) Dec-21              30) Jan-04
    #?
    ```
Here we can see I got nothin goin on until March. Heh.
* When you select a folder, you are dropped to a shell with the PWD set to the
  proper directory. Suggestions: Add a TODO file! Copy those meetings notes
  over! Whatever!
* If today's folder isn't empty, open that bad boy up and copy the TODO contents
  to your organizer. Or whatever.

Like I said, low-tech.
