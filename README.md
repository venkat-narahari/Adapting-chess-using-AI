# Adapting-chess-using-AI
The code is almost entirely ANSI compliant, with one or two
exceptions.  There is very little file handling, and at the moment, only a
very small number of complicated features.  Beowulf runs in text mode, and
is also fully compatible with Xboard/Winboard graphical interfaces.

In order to install, the source must be compiled.most efficient compile option is simply to compile the source include file
chess.c on its own with full optimisations.  i.e. for systems using GCC
as their primary compiler, type;

The configuration file (beowulf.cfg) should be left in the install directory.
Whenever Beowulf is run from that directory, the configuration file is read
in order to overwrite the default options in the source.

Finally, a set of command line options can also be issued.  These override
all other settings, and are useful for setting the hash table size for use
in test games.  For a list, try running Beowulf with the command line option
'--help'.  The list is reproduced here for your benefit;

?, help            - Print this file
hash<num>          - Set the hash table size (2^n kb)
tbloc=<directory>  - Set the tablebase location
book=<filename>    - Set the opening book
person=<filename>  - Set the personality file
wskill<num>        - Set the skill level for white (1 to 10)
bskill<num>        - Set the skill level for black (1 to 10)
epdtest=<file>     - Run an EPD test and quit immediately
st<num>            - Set the time per move for an EPD test (default 5s)
