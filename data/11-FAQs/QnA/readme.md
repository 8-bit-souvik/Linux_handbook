## Difference between Bash, Shell, UXTerm and Terminal and other shells

In linux they can all look the same from the point of view of the user at the keyboard. The differences are in how they interact with each other.

The shell is the program which actually processes commands and returns output. Most shells also manage foreground and background processes, command history and command line editing. These features (and many more) are standard in <b>`bash (bourn again shell)`</b>, the most common shell in modern linux systems.
there is a lot other shells exists like -
- Bourne shell (sh)
- C shell (csh)
- TC shell (tcsh)
- Korn shell (ksh)

```
                    Bourne   C    TC   Korn   BASH
________________________________________________________


command history        No   Yes   Yes   Yes    Yes

command alias          No   Yes   Yes   Yes    Yes

shell scripts          Yes  Yes   Yes   Yes    Yes

filename completion    No   Yes*  Yes   Yes*   Yes

command line editing   No   No    Yes   Yes*   Yes

job control            No   Yes   Yes   Yes    Yes
________________________________________________________

* not the default setting for this shell

```

A <b>`terminal`</b> refers to a wrapper program which runs a shell. Decades ago, this was a physical device consisting of little more than a monitor and keyboard. As unix/linux systems added better multiprocessing and windowing systems, this terminal concept was abstracted into software. Now you have programs such as Gnome Terminal which launches a window in a Gnome windowing environment which will run a shell into which you can enter commands.

<b>UXTerm</b>, <b>XTerm</b>, <b>Konsole</b>, <b>rxvt</b> and a bunch of others are examples of terminal programs.

<b>`UXTerm`</b> is XTerm with support to Unicode characters. The main difference between XTerm and Terminal is that the gnome-terminal has more features, while XTerm is minimalistic (though it has features that are't in gnome-terminal, but they are more advanced).
