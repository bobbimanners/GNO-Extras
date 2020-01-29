**UNIX v7 Userspace Goodies for the GNO/ME 2.0.6 ORCA/C 2.2.0B3 Environment**

I have ported a number of utilities and games from UNIX version 7
(1979 release for the PDP-11) to the GNO/ME environment running on
the Apple IIgs.  All of these programs build with the ORCA/C 2.2.0B3
compiler.

*Utilities*

These install into `/usr/local/bin`.  Man pages are provided and install into
`/usr/local/man/man1`.

- `cal` - Displays a calendar.
- `dd` - Disk dumper - convert and copy a file.
- `find` - Search for files in directory hierarchy.
- `file` - Determine file type.
- `od` - Dump files in octal and other formats.
- `rev` - Reverse lines characterwise.
- `units` - Convert between different units of measure.

*Games*

These install into `/usr/local/games`.

- `arithmetic` - Arithmetic exercise.
- `backgammon` - Backgammon.
- `fish` - Go Fish!
- `fortune` - Fortune cookie.
- `hangman` - Hangman.
- `quiz` - Quiz with various categories.
- `wump` - Hunt the Wumpus.

*Licence*

Caldera issued a free licence in 2002 covering the 'ancient UNIX' code including version 7.
This licence allows use, modification and distribution of the code.

Any original work here is licenced under the BSD 2 clause licence.

*Build Instructions*

Under GNO, issue the following commands:

```
cd v7/cmd
dmake
dmake install
cd ../games
dmake
dmake install
```

*Disclaimer / To Do*

`backgammon` and `quiz` do not work yet.

Very minimal testing has been performed.  If you find bugs, please let me know!

I plan to port more version 7 utilities in due course.
